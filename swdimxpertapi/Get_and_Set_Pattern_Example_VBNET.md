<!-- source: swdimxpertapi/Get_and_Set_Pattern_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Get and Set Pattern Example (VB.NET)

This example shows how to get
and set DimXpert pattern features.

'---------------------------------------------------------------------------
' Preconditions:
' 1. Open: *public\_documents***\samples\tutorial\dimxpert\bracket\_auto\_manual.sldprt.**
' 2. Select one of the CBORE hole faces in the SOLIDWORKS viewer.
' 3. Open an Immediate window.
' 4. Ensure that the latest SOLIDWORKS DimXpert interop assembly is
referenced:
'    a. Right-click the project in Project Explorer.
'    b. Select **Add Reference**.
'    c. Click the Browse tab.
'    d. Find and select *install\_dir***\api\redist\swdimxpert.dll**.

'
' Postconditions: Inspect the Immediate window and the DimXpertManager tab.
'
' NOTE: Because this part is used elsewhere, do not save changes.
'--------------------------------------------------------------------------
Imports
SolidWorks.Interop.sldworks
Imports
SolidWorks.Interop.swconst
Imports
SolidWorks.Interop.swdimxpert
Imports
System
Imports
System.Diagnostics

Partial
Class
SolidWorksMacro

    Dim
dimXpertPart As
dimXpertPart
    Dim
swModelDoc As
ModelDoc2
    Dim
featureType As
swDimXpertFeatureType\_e
    Dim
msgStr As
String
    Dim
msgStr2 As
String
    Dim
msgStr3 As
String
    Dim
n As
Long
    Dim
retval As
Boolean

    Sub
Main()

        swModelDoc = swApp.ActiveDoc

        If
swModelDoc Is
Nothing
Then
            Exit
Sub
        End
If

        Dim
dimXpertMgr As
DimXpertManager
        dimXpertMgr =
swApp.IActiveDoc2.Extension.DimXpertManager(swApp.IActiveDoc2.IGetActiveConfiguration().Name,
True)
        Debug.Print("Model: "
& swApp.IActiveDoc2.GetPathName)

        Dim
dimXpertPartObj As
dimXpertPart
        dimXpertPartObj = dimXpertMgr.dimXpertPart
        dimXpertPart = dimXpertPartObj

        Dim
selectMgr As
SelectionMgr
        selectMgr = swApp.IActiveDoc2.SelectionManager

        Dim
dimOption As
DimXpertDimensionOption
        dimOption = dimXpertPart.**GetDimOption**

        Dim
patternType As
Long
        patternType = 2
' collection pattern

        Dim
findall As
Boolean
        findall =
True
' find all similar features on this face

        Dim
dimarray(0) As
Long
        dimarray(0) = -1  '
default
        Dim
dimvar As
Object
        dimvar = dimarray
        dimOption.**FeatureSelectorOptions** = dimvar

' Mark the current selection with an index value
greater than 50
        retval = selectMgr.SetSelectedObjectMark(1, 51,
swSelectionMarkAction\_e.swSelectionMarkSet)

        ' Insert the collection pattern
feature
        retval =
dimXpertPart.**InsertPattern**(dimOption, patternType, findall)

        Dim
featCount As
Long
        featCount =
dimXpertPart.GetFeatureCount

        If
Not (featCount
= 0) Then

            Dim
patternFeature As
IDimXpertPatternFeature
            patternFeature = dimXpertPart.GetFeature("Collection1")

            msgStr = patternFeature.**Name** +
" is a DimXpert collection pattern feature."
            Debug.Print("")
            Debug.Print(msgStr)

            featureType = patternFeature.**patternType**

            Call
GetPatternType(featureType, msgStr2)

            Dim
featureCount As
Integer

            featureCount =
patternFeature.**GetSubFeatureCount**()
            msgStr = "     Number of "
            msgStr3 = featureCount
            Debug.Print(msgStr + msgStr2 +
" sub-features in this pattern is "
+ msgStr3)

            Dim
subfeatures As
Object
            subfeatures =
patternFeature.**GetSubFeatures**()

            Debug.Print("
Sub-features of Collection1:")
            Dim
subFeature As
DimXpertCompoundHoleFeature

            For
n = 0 To
UBound(subfeatures)
                subFeature = subfeatures(n)
                Debug.Print("        "
+ subFeature.Name)
            Next

        Else
            Debug.Print("Please
select a CBORE hole face in the viewer and run this macro again.")

        End
If

    End
Sub

    Public
Sub
GetPatternType(ByRef
featureType As
swDimXpertFeatureType\_e, ByRef
msgStr2 As
String)

        If
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_Plane)
Then
            msgStr2 =
"Plane"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_Cylinder)
Then
            msgStr2 =
"Cylinder"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_Cone)
Then
            msgStr2 =
"Cone"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_Extrude)
Then
            msgStr2 =
"Extrude"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_Fillet)
Then
            msgStr2 =
"Fillet"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_Chamfer)
Then
            msgStr2 =
"Chamfer"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundHole)
Then
            msgStr2 =
"CompoundHole"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundWidth)
Then
            msgStr2 =
"CompoundWidth"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundNotch)
Then
            msgStr2 =
"CompoundNotch"

        ElseIf
(featureType =
swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundClosedSlot3D)
Then
            msgStr2 =
"CompoundClosedSlot3D"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectPoint)
Then
            msgStr2 =
"IntersectPoint"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectLine)
Then
            msgStr2 =
"IntersectLine"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectCircle)
Then
            msgStr2 =
"IntersectCircle"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectPlane)
Then
            msgStr2 =
"IntersectPlane"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_Pattern)
Then
            msgStr2 =
"Pattern"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_Sphere)
Then
            msgStr2 =
"Sphere"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_BestfitPlane)
Then
            msgStr2 =
"Bestfit plane"

        ElseIf
(featureType = swDimXpertFeatureType\_e.swDimXpertFeature\_Surface)
Then
            msgStr2 =
"Surface"

        End
If

    End
Sub

    Public
swApp As
SldWorks

End
Class