<!-- source: sldworksapi/Add_and_Delete_Materials_from_Specific_Display_States_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Add and Delete Appearances from Specific Display States Example (C#)

This example shows how to add an appearance to and delete an appearance from specific
display states.

//---------------------------------------------------------------------------

// Preconditions:

// 1. Specified model exists.

// 2. Specified appearance exists.

// 3. Open an Immediate window.

//

// Postconditions:

// 1. Creates Display State 2 and Display State 3 for the
active

//    configuration.

// 2. Applies specified appearance to all display states of the
active

//    configuration.

// 3. Press F5.

// 4. Deletes specified appearance from all display states of
the active

//    configuration.

// 5. Press F5.

// 6. Closes document.

//---------------------------------------------------------------------------

using

 Microsoft.VisualBasic;

using

 System;

using

 System.Collections;

using

 System.Collections.Generic;

using

 System.Data;

using

 System.Diagnostics;

using

 SolidWorks.Interop.sldworks;

using

 SolidWorks.Interop.swconst;

using

 System.Runtime.InteropServices;

namespace

 RenderMaterials\_CSharp.csproj

{

partial class
SolidWorksMacro

    {

ModelDoc2
swModel;Configuration
swConfig;
ModelDocExtension swModelDocExt;Entity
swEntity;SelectionMgr
swSelMgr;RenderMaterial
swRenderMaterial;object[]
displayStateNames;bool
status;string
modelName;string
materialName;int
errors;int
warnings;int
nbrDisplayStates;int
i;int
k;int
nbrMaterials;int
materialID1;int
materialID2;int[]
materialID1\_ToDelete = new
int[1];int[]
materialID2\_ToDelete = new
int[1];public
void Main()

{

> modelName =

"C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2018\\samples\\tutorial\\dimxpert\\bracket\_auto\_manual.sldprt";

swModel = swApp.**OpenDoc6**(modelName, (

int)swDocumentTypes\_e.swDocPART,
(int)swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"",
ref
errors, ref
warnings);

swModelDocExt = swModel.**Extension**;

// Get
active configuration and create a new display
// state
for this configuration

swConfig = (

Configuration)swModel.**GetActiveConfiguration**();

status = swConfig.**CreateDisplayState**(

"Display
State 2");

swModel.**ForceRebuild3**(

true);// Get
active configuration and create another new
// display
state for this configuration

swConfig = (

Configuration)swModel.**GetActiveConfiguration**();

status = swConfig.**CreateDisplayState**(

"Display
State 3");

swModel.**ForceRebuild3**(

true);// Create
appearance

materialName =

"C:\\Program Files\\SolidWorks Corp\\SolidWorks\\data\\graphics\\materials\\metal\\steel\\stainless
steel treadplate.p2m";

swRenderMaterial = swModelDocExt.**CreateRenderMaterial**(materialName);

// Select a
face and add the appearance to that face

status = swModelDocExt.**SelectByID2**(

"",
"FACE",
0.07151920610502, 0.0952597996959, 0.009524999999996,
false, 0,
null,
0);

swSelMgr = (

SelectionMgr)swModel.**SelectionManager**;

swEntity = (

Entity)swSelMgr.**GetSelectedObject6**(1,
-1);

status = swRenderMaterial.**AddEntity**(swEntity);

// Get the
names of display states

displayStateNames = (

object[])swConfig.**GetDisplayStates**();

nbrDisplayStates = swConfig.**GetDisplayStatesCount**();

Debug.Print("This
configuration's display states =");for
(i = 0; i <= (nbrDisplayStates - 1); i++)

{

Debug.Print("
Display state name = " + displayStateNames[i]);

}

// Add
appearance to all of the display states

status = swModelDocExt.**AddDisplayStateSpecificRenderMaterial**(swRenderMaterial,
(

int)swDisplayStateOpts\_e.swAllDisplayState,
displayStateNames, out
materialID1, out
materialID2);// Get the
appearance IDs and names

swRenderMaterial.**GetMaterialIds**(

out
materialID1, out
materialID2);Debug.Print("
Appearance IDs:");Debug.Print("
ID1 = " + materialID1);Debug.Print("
ID2 = " + materialID2);

nbrMaterials = swModelDocExt.**GetRenderMaterialsCount2**((

int)swDisplayStateOpts\_e.swAllDisplayState,
null);Debug.Print("
Number of materials: " + nbrMaterials);for
(k = 0; k <= (nbrMaterials - 1); k++)

{

Debug.Print("
Name of appearance " + (k + 1) +
": " + swModel.**MaterialIdName**);

}

double
xcoord = 0;double
ycoord = 0;double
zcoord = 0;

swRenderMaterial.**GetCenterPoint2**(

out
xcoord, out
ycoord, out
zcoord);Debug.Print("");Debug.Print("Texture-based
appearance data:");Debug.Print("X
coordinate of center point: " + xcoord);Debug.Print("Y
coordinate of center point: " + ycoord);Debug.Print("Z
coordinate of center point: " + zcoord);

swRenderMaterial.**GetUDirection2**(

out
xcoord, out
ycoord, out
zcoord);Debug.Print("X
coordinate of U direction: " + xcoord);Debug.Print("Y
coordinate of U direction: " + ycoord);Debug.Print("Z
coordinate of U direction: " + zcoord);

swRenderMaterial.**GetVDirection2**(

out
xcoord, out
ycoord, out
zcoord);Debug.Print("X
coordinate of V direction: " + xcoord);Debug.Print("Y
coordinate of V direction: " + ycoord);Debug.Print("Z
coordinate of V direction: " + zcoord);Debug.Print("");

swModel.**ClearSelection2**(

true);

swModel.**ForceRebuild3**(

true);Debug.Print("Model
has an appearance: " + swModelDocExt.**HasMaterialPropertyValues**());object
dispStates = null;

status = swRenderMaterial.**SetLinkedDisplayStates**((

int)swDisplayStateOpts\_e.swAllDisplayState,
displayStateNames);

dispStates = swRenderMaterial.**GetLinkedDisplayStates**();

object
renderMaterials = null;

renderMaterials = swModelDocExt.**GetRenderMaterials2**((

int)swDisplayStateOpts\_e.swAllDisplayState,
null);// Examine
the display states of the active configuration
// to
ensure that the specified appearance was applied to all
// display
states
// Continue
running the macro after your examination

System.Diagnostics.

Debugger.Break();// Delete
the appearance from the part

materialID1\_ToDelete[0] = materialID1;

materialID2\_ToDelete[0] = materialID2;

swModelDocExt.**DeleteDisplayStateSpecificRenderMaterial**((materialID1\_ToDelete),
(materialID2\_ToDelete));

swModel.**ForceRebuild3**(

true);// Examine
the display states of the active configuration
// to
ensure that the specified appearance was deleted from all
// display
states
// Continue
running the macro after your examination

System.Diagnostics.

Debugger.Break();// Close
the part without saving changes

modelName = swModel.**GetTitle**();

swApp.**QuitDoc**(modelName);

}

public SldWorks
swApp;

        }

}