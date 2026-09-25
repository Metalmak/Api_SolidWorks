<!-- source: sldworksapi/Mirror_Components_II_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Mirror Components II Example (VB.NET)

This example shows how to mirror components in an assembly.

'---------------------------------------------------------------------------------

'
Preconditions:

' 1. Open
**C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS
2020\samples\tutorial\advdrawings\98food processor.sldasm**.

' 2.
Ensure that **c:\API\MirrorComps** exists.

'
Postconditions:

' 1.
Creates **Plane4** mirror plane.

' 2.
Creates mirror copies of **gear- caddy-1** and **middle-gear-1**, both aligned to
component origins.

' 3.
Creates mirror copies of **shaft gear-1** and **middle-gear plate-1**, aligned to
**PLANE2** and **PLANE3**, respectively.

' 4.
Creates opposite-hand versions of **base plate-1** and **shaft gear insert-1**,
called **FileName1.sldprt** and **FileName2.sldprt**, respectively, and stored in
**c:\API\MirrorComps**.

' 5.
Replaces **FileName1.sldprt** with **check1.sldprt**in **c:\API\MirrorComps**.

' 6.
Creates **MirrorComponent1** in the FeatureManager design tree.

' 7.
Modifies **MirrorComponent1** to change the mirror type, the align to origin
component orientations, and the align to selection orientations.

'

' NOTE:
Because the model is used elsewhere, do not save any changes to it.

'---------------------------------------------------------------------------------------

Imports SolidWorks.Interop.sldworks

Imports SolidWorks.Interop.swconst

Imports System.Runtime.InteropServices

Imports System

Partial
Class
SolidWorksMacro

Dim swModel
As
ModelDoc2

Dim swAssem
As
AssemblyDoc

Dim swFeat
As
Feature

Dim mirrorPlane
As
Feature

Dim FeatMgr
As
FeatureManager

Dim swMirroCompFeatData
As
MirrorComponentFeatureData

Dim myRefPlane
As
RefPlane

Dim compsToMirrorOrientationonOrigin(1)
As

swMirrorComponentOrientation2\_e

Dim compsToMirrorOrientationonPlane(1)
As
swMirrorComponentOrientation2\_e

Dim mirrorPlane2
As
Feature

Dim mirrorPlane3
As
Feature

Dim FlipDir(1)
As
Boolean

Dim flipDirVar
As
Object

Dim orientationArray
As
Object

Dim orientationSelPlanArray
As
Object

Dim mirrorCompFileNames(1)
As
String

Dim mirrorCompFolder
As
String

Dim namesVar
As
Object

Dim replaceLocations(1)
As
String

Dim replaceLocationsArray
As
Object

Dim importOptions
As
Integer

Dim modifyFeatdef
As
MirrorComponentFeatureData

Dim compsToMirrorOrientationonOrigin2(1)
As

swMirrorComponentOrientation2\_e

Dim compsToMirrorOrientationonPlane2(1)
As

swMirrorComponentOrientation2\_e

Dim orientationArray2
As
Object

Dim orientationArrayPlane2
As
Object

Dim swCompInst
As
Object =
Nothing

Dim CTI(1)
As
DispatchWrapper

Dim CTSP(1)
As
DispatchWrapper

Dim CTMOH(1)
As
DispatchWrapper

Dim ARef(1)
As
DispatchWrapper

Dim boolstatus
As
Boolean

Dim retVal
As
Boolean

Sub main()

swModel = swApp.ActiveDoc

FeatMgr = swModel.FeatureManager

' Create mirror
component feature data object

swMirroCompFeatData = FeatMgr.**CreateDefinition**(swFeatureNameID\_e.swFmMirrorComponent)

' Create mirror
plane

boolstatus = swModel.Extension.SelectByID2("",
"FACE", 0.104250921669188, -0.000236987012272039, -0.0597199999999418,
True, 0,
Nothing, 0)

myRefPlane = swModel.FeatureManager.InsertRefPlane(8, 0.01, 0, 0, 0,
0)

swAssem = swModel

mirrorPlane = swAssem.FeatureByName("PLANE4")

' Specify
components to instance align to component origins

swCompInst = swAssem.GetComponentByName("gear- caddy-1")

CTI(0) =
New
DispatchWrapper(swCompInst)

swCompInst = swAssem.GetComponentByName("middle-gear-1")

CTI(1) =
New
DispatchWrapper(swCompInst)

' Specify
components to instance align to alignment references

swCompInst = swAssem.GetComponentByName("shaft gear-1")

CTSP(0) =
New

DispatchWrapper(swCompInst)

swCompInst = swAssem.GetComponentByName("middle-gear plate-1")

CTSP(1) =
New

DispatchWrapper(swCompInst)

' Specify
components for which to create new opposite-hand versions

swCompInst = swAssem.GetComponentByName("base plate-1")

CTMOH(0) =
New

DispatchWrapper(swCompInst)

swCompInst = swAssem.GetComponentByName("shaft gear insert-1")

CTMOH(1) =
New

DispatchWrapper(swCompInst)

' Specify align
to origins component orientations

compsToMirrorOrientationonOrigin(0) =
swMirrorComponentOrientation2\_e.swOrientation\_MirroredX\_MirroredY

compsToMirrorOrientationonOrigin(1) =
swMirrorComponentOrientation2\_e.swOrientation\_MirroredAndFlippedX\_MirroredY

orientationArray = compsToMirrorOrientationonOrigin

' Specify align
to selection component orientations

compsToMirrorOrientationonPlane(0) =
swMirrorComponentOrientation2\_e.swOrientation\_MirroredX\_MirroredAndFlippedY

compsToMirrorOrientationonPlane(1) =
swMirrorComponentOrientation2\_e.swOrientation\_MirroredAndFlippedX\_MirroredAndFlippedY

orientationSelPlanArray = compsToMirrorOrientationonPlane

' Specify the
alignment references for the align to selection components

mirrorPlane2 = swAssem.FeatureByName("PLANE2")

ARef(0) =
New

DispatchWrapper(mirrorPlane2)

mirrorPlane3 = swAssem.FeatureByName("PLANE3")

ARef(1) =
New

DispatchWrapper(mirrorPlane3)

' Specify
whether to reverse the direction of alignment

FlipDir(0) =
False

FlipDir(1) =
False

flipDirVar = FlipDir

' Specify the
opposite-hand version folder

mirrorCompFolder =
"C:\API\MirrorComps"

' Specify
opposite-hand version file names

mirrorCompFileNames(0) = ("FileName1")

mirrorCompFileNames(1) = ("FileName2")

namesVar = mirrorCompFileNames

' Specify
replacement locations for the opposite-hand versions

replaceLocations(0) = ("C:\API\check1.SLDPRT")

replaceLocations(1) = ("")

replaceLocationsArray = replaceLocations

' Specify
transfer options for the opposite-hand versions

importOptions =
swMirrorPartOptions\_e.swMirrorPartOptions\_ImportSolids

swMirroCompFeatData.**mirrorPlane** = mirrorPlane

swMirroCompFeatData.**MirrorType** =
swMirrorComponentMirrorType\_e.swMirrorType\_ComponentOrigin

swMirroCompFeatData.**ComponentsToInstanceAlignToComponentOrigin** = CTI

swMirroCompFeatData.**ComponentOrientationsAlignToComponentOrigin** =
orientationArray

swMirroCompFeatData.**ComponentsToInstanceAlignToSelection** = CTSP

swMirroCompFeatData.**ComponentOrientationsAlignToSelection** =
orientationSelPlanArray

swMirroCompFeatData.**AlignmentReferences** = ARef

swMirroCompFeatData.**FlipDirections** = flipDirVar

swMirroCompFeatData.**SyncFlexibleSubAssemblies** =
True

swMirroCompFeatData.**OppositeHandComponents** = CTMOH

swMirroCompFeatData.**CreateDerivedConfigurations** =
False

swMirroCompFeatData.**PlaceFilesInOneFolder** =
True

swMirroCompFeatData.**MirrorComponentsFolderLocation** = mirrorCompFolder

swMirroCompFeatData.**MirroredComponentFilenames** = namesVar

swMirroCompFeatData.**MirroredComponentFilenames** = mirrorCompFileNames

swMirroCompFeatData.**NameModifierType** =
swMirrorComponentNameModifier\_e.swMirrorComponentName\_Custom

swMirroCompFeatData.**ReplaceFileLocations** = replaceLocationsArray

swMirroCompFeatData.**MirrorTransferOptions** = importOptions

swMirroCompFeatData.**DimXpertScheme** =
True

swMirroCompFeatData.**BreakLinksToOriginalPart** =
False

swMirroCompFeatData.**preserveZAxis** =
True

swMirroCompFeatData.**PropagateFromOriginalPart** =
False

' Create
MirrorComponent1

swFeat = FeatMgr.**CreateFeature**(swMirroCompFeatData)

' Modify
MirrorComponent1

modifyFeatdef = swFeat.**GetDefinition**

' Change mirror
type to center of mass

modifyFeatdef.**MirrorType** =
swMirrorComponentMirrorType\_e.swMirrorType\_CenterOfMass

' Modify align
to origin component orientations

compsToMirrorOrientationonOrigin2(0) =
swMirrorComponentOrientation2\_e.swOrientation\_MirroredAndFlippedX\_MirroredAndFlippedY

compsToMirrorOrientationonOrigin2(1) =
swMirrorComponentOrientation2\_e.swOrientation\_MirroredX\_MirroredAndFlippedY

orientationArray2 = compsToMirrorOrientationonOrigin2

modifyFeatdef.**ComponentOrientationsAlignToComponentOrigin** =
orientationArray2

' Modify align
to selection component orientations

compsToMirrorOrientationonPlane2(0) =
swMirrorComponentOrientation2\_e.swOrientation\_MirroredAndFlippedX\_MirroredY

compsToMirrorOrientationonPlane2(1) =
swMirrorComponentOrientation2\_e.swOrientation\_MirroredX\_MirroredY

orientationArrayPlane2 = compsToMirrorOrientationonPlane2

modifyFeatdef.**ComponentOrientationsAlignToSelection** =
orientationArrayPlane2

retVal = swFeat.**ModifyDefinition**(modifyFeatdef, swModel,
Nothing)

End
Sub

'''
<summary>

''' The SldWorks swApp variable is pre-assigned for you.

'''
</summary>

Public swApp
As
SldWorks

End
Class