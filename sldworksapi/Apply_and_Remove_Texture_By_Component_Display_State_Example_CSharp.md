<!-- source: sldworksapi/Apply_and_Remove_Texture_By_Component_Display_State_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Apply and Remove Texture To and From Component By Display State (C#)

This example shows how to apply and remove texture to and from a component
using the name of a display state of the model.

```
//-------------------------------------------------------------------------
// Preconditions:
// 1. Verify that the specified assembly to open and texture exist.
// 2. Open the Immediate window.
//
// Postconditions:
// 1. Opens the specified assembly and applies texture to
//    the selected component.
// 2. Examine the Immediate window.
// 3. Click anywhere in the SOLIDWORKS window
//    to verify that the texture was applied.
// 4. Follow the instructions in the macro
//    to remove the just-applied texture.
// 5. Run the macro again.
// 6. Examine the Immediate window.
// 7. Click anywhere in the SOLIDWORKS window to verify
//    that the texture was removed.
//
// NOTE: Because this assembly document is used elsewhere,
// do not save changes.
//---------------------------------------------------------------------------
using
```

 SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using System;
using System.Diagnostics;

namespace

ApplyRemoveTextureByDisplayStateCSharp.csproj

{

partial class
SolidWorksMacro

    {

public void
Main()

        {

ModelDoc2
swModel = default(ModelDoc2);
SelectionMgr swSelMgr =
default(SelectionMgr);
ModelDocExtension swModelDocExt =
default(ModelDocExtension);Component2
component = default(Component2);Texture
texture = default(Texture);bool
status = false;string
displayState = null;int
errors = 0;int
warnings = 0;string
namStr = null;

// Open document
and select a component

swModel = (

ModelDoc2)swApp.**OpenDoc6**("C:\\Users\\Public\\Documents\\SOLIDWORKS\SOLIDWORKS
2018\\samples\\tutorial\\motionstudies\\valve\_cam.sldasm",
(int)swDocumentTypes\_e.swDocASSEMBLY,
(int)swOpenDocOptions\_e.**swOpenDocOptions\_Silent**,
"",
ref
errors, ref
warnings);

swModelDocExt = (

ModelDocExtension)
swModel.Extension;

status = swModelDocExt.**SelectByID2**(

"rocker-1@valve\_cam",
"COMPONENT",
0, 0, 0, false,
0, null,
0);

swSelMgr = (

SelectionMgr)swModel.**SelectionManager**;

component = (

Component2)
swSelMgr.**GetSelectedObject6**(1, -1);

displayState =

"Default\_Display State-1";

namStr =

"<SystemTexture>\\images\\textures\\pattern\\checker2.jpg";

// Set texture on
selected component in the

// specified
display state

// After
running the macro the first time, edit the macro to

// insert
the comment characters (//) before the following two
// lines of
code

texture = (

Texture)
swModelDocExt.**CreateTexture**(namStr, 5, 45,
false);Debug.Print
("Texture set: "
+ component.**SetTextureByDisplayState**(displayState, texture));
// Remove
texture from component by display state // After
running the macro the first time, edit it to
// remove
the comment characters (//) before the following
// line of
code
//Debug.Print
("Texture removed: " + component.**RemoveTextureByDisplayState**(displayState));

        }

///
<summary>

///
The SldWorks swApp variable is pre-assigned for you.
///
</summary>

public
SldWorks swApp;

    }

}