<!-- source: sldworksapi/Add_and_Delete_Materials_from_Specific_Display_States_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Add and Delete Appearances from Specific Display States Example (VB.NET)

This example shows how to add an appearance to and delete an appearance from specific
display states.

'---------------------------------------------------------------------------

' Preconditions:

' 1. Specified model exists.

' 2. Specified appearance exists.

' 3. Open an Immediate window.

'

' Postconditions:

' 1. Creates Display State 2 and Display State 3 for the
active

'    configuration.

' 2. Applies specified appearance to all display states of the
active

'    configuration.

' 3. Press F5.

' 4. Deletes specified appearance from all display states of
the active

'    configuration.

' 5. Press F5.

' 6. Closes document.

'---------------------------------------------------------------------------

Imports

 SolidWorks.Interop.sldworks

Imports

 SolidWorks.Interop.swconst

Imports

 System.Runtime.InteropServices

Imports

 System

Imports

 System.Diagnostics

Partial

Class SolidWorksMacro
Dim
swModel As
ModelDoc2Dim
swConfig As
ConfigurationDim
swModelDocExt As
ModelDocExtensionDim
swEntity As
EntityDim
swSelMgr As
SelectionMgrDim
swRenderMaterial As
RenderMaterialDim
displayStateNames As
Object
Dim
status As
Boolean
Dim
modelName As
String
Dim
materialName As
String
Dim
errors As
Integer
Dim
warnings As
Integer
Dim
nbrDisplayStates As
Integer
Dim
i As
Integer
Dim
k As
Integer
Dim
nbrMaterials As
Integer
Dim
materialID1 As
Integer
Dim
materialID2 As
Integer
Dim
materialID1\_ToDelete(0) As
Integer
Dim
materialID2\_ToDelete(0) As
Integer
Sub
main()
> modelName =

"C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2018\samples\tutorial\dimxpert\bracket\_auto\_manual.sldprt"

swModel = swApp.**OpenDoc6**(modelName,
swDocumentTypes\_e.swDocPART, swOpenDocOptions\_e.swOpenDocOptions\_Silent,

"", errors,
warnings)

swModelDocExt = swModel.**Extension**

' Get active
configuration and create a new display
' state for
this configuration

swConfig = swModel.**GetActiveConfiguration**

status = swConfig.**CreateDisplayState**(

"Display
State 2")

swModel.**ForceRebuild3**(

True)' Get active
configuration and create another new
' display state
for this configuration

swConfig = swModel.**GetActiveConfiguration**

status = swConfig.**CreateDisplayState**(

"Display
State 3")

swModel.**ForceRebuild3**(

True)' Create
appearance

materialName =

"C:\Program Files\SolidWorks Corp\SolidWorks\data\graphics\materials\metal\steel\stainless
steel treadplate.p2m"

swRenderMaterial = swModelDocExt.**CreateRenderMaterial**(materialName)

' Select a face
and add the appearance to that face

status = swModelDocExt.**SelectByID2**(

"",
"FACE",
0.07151920610502, 0.0952597996959, 0.009524999999996,
False, 0,
Nothing, 0)

swSelMgr = swModel.**SelectionManager**

swEntity = swSelMgr.**GetSelectedObject6**(1, -1)

status = swRenderMaterial.**AddEntity**(swEntity)

' Get the names
of display states

displayStateNames = swConfig.**GetDisplayStates**

nbrDisplayStates = swConfig.**GetDisplayStatesCount**

Debug.Print(

"This
configuration's display states =")For
i = 0 To (nbrDisplayStates
- 1)

Debug.Print(

"
Display state name = " & displayStateNames(i))Next
i' Add
appearance
to all of the display states

status = swModelDocExt.**AddDisplayStateSpecificRenderMaterial**(swRenderMaterial,
swDisplayStateOpts\_e.swAllDisplayState, displayStateNames, materialID1,
materialID2)

' Get the
appearance IDs and names

swRenderMaterial.**GetMaterialIds**(materialID1,
materialID2)

Debug.Print(

"
Appearance IDs:")

Debug.Print(

"
ID1 = " & materialID1)

Debug.Print(

"
ID2 = " & materialID2)

nbrMaterials = swModelDocExt.**GetRenderMaterialsCount2**(swDisplayStateOpts\_e.swAllDisplayState,

Nothing)

Debug.Print(

"
Number of appearances: " & nbrMaterials)For
k = 0 To (nbrMaterials
- 1)

Debug.Print(

"
Name of appearance " & (k + 1) &
": " & swModel.**MaterialIdName**)Next
kDim
xcoord As
Double
Dim
ycoord As
Double
Dim
zcoord As
Double

swRenderMaterial.**GetCenterPoint2**(xcoord,
ycoord, zcoord)

Debug.Print(

"")

Debug.Print(

"Texture-based
appearance data:")

Debug.Print(

"X
coordinate of center point: " & xcoord)

Debug.Print(

"Y
coordinate of center point: " & ycoord)

Debug.Print(

"Z
coordinate of center point: " & zcoord)

swRenderMaterial.**GetUDirection2**(xcoord, ycoord,
zcoord)

Debug.Print(

"X
coordinate of U direction: " & xcoord)

Debug.Print(

"Y
coordinate of U direction: " & ycoord)

Debug.Print(

"Z
coordinate of U direction: " & zcoord)

swRenderMaterial.**GetVDirection2**(xcoord, ycoord,
zcoord)

Debug.Print(

"X
coordinate of V direction: " & xcoord)

Debug.Print(

"Y
coordinate of V direction: " & ycoord)

Debug.Print(

"Z
coordinate of V direction: " & zcoord)

Debug.Print(

"")

swModel.**ClearSelection2**(

True)

swModel.**ForceRebuild3**(

True)

Debug.Print(

"Model
has an appearance: " & swModelDocExt.**HasMaterialPropertyValues**)Dim
dispStates As
Object

status = swRenderMaterial.**SetLinkedDisplayStates**(swDisplayStateOpts\_e.swAllDisplayState,
displayStateNames)

dispStates = swRenderMaterial.**GetLinkedDisplayStates**

Dim
renderMaterials As
Object

renderMaterials = swModelDocExt.**GetRenderMaterials2**(swDisplayStateOpts\_e.swAllDisplayState,

Nothing)' Examine the
display states of the active configuration
' to ensure
that the specified appearance was applied to all
' display
states' Continue
running the macro after your examination
Stop
' Delete the
appearance from the part

materialID1\_ToDelete(0) = materialID1

materialID2\_ToDelete(0) = materialID2

swModelDocExt.**DeleteDisplayStateSpecificRenderMaterial**((materialID1\_ToDelete),
(materialID2\_ToDelete))

swModel.ForceRebuild3(

True)' Examine the
display states of the active configuration
' to ensure
that the specified appearance was deleted from all
' display
states
' Continue
running the macro after your examination
Stop
' Close the
part without saving changes

modelName = swModel.**GetTitle**

swApp.**QuitDoc**(modelName)

    End
Sub
Public swApp As
SldWorks

End

Class