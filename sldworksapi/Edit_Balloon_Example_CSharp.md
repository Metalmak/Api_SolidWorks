<!-- source: sldworksapi/Edit_Balloon_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Edit Balloon Example (C#)

This example shows how to edit a balloon in a drawing document.

//
--------------------------------------------------------------------------
// Preconditions:
// 1. Open *public\_documents***\samples\tutorial\advdrawings\foodprocessor.slddrw.**
// 2. Click **Insert > Annotations > Balloon**.
// 3. Click a model edge in either drawing view and add the balloon.
// 4. Close the Balloon PropertyManager page.
// 5. Select the balloon in the drawing.
//
// Postconditions: The properties of the selected balloon are modified.
//
// **NOTE:** Because this drawing document is used elsewhere, do not save any
// changes when closing it.
//
--------------------------------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System.Runtime.InteropServices;
using
System;
using
System.Diagnostics;
namespace
EditBalloonProperties\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {
        ModelDoc2
swModel;
        ModelDocExtension
swModelDocExt;
        SelectionMgr
swSelMgr;
        Note
swNote;

        public
void Main()
        {
            swModel = (ModelDoc2)swApp.**ActiveDoc**;
            swModelDocExt = swModel.**Extension**;
            swSelMgr = (SelectionMgr)swModel.**SelectionManager**;

            // Get the selected balloon
            swNote = (Note)swSelMgr.**GetSelectedObject6**(1,
-1);

            // Edit the selected balloon
            swNote = (Note)swModelDocExt.**EditBalloonProperties2**((int)swBalloonStyle\_e.swBS\_SplitCirc,
(int)swBalloonFit\_e.swBF\_5Chars,
(int)swBalloonTextContent\_e.swBalloonTextCustom,
"Upper",
(int)swBalloonTextContent\_e.swBalloonTextCustom,
"Lower",
0, true, 1,
"X",
            0.0355);

            Debug.Print("Balloon
name:  " + swNote.**GetName**());
        }

        public
SldWorks
swApp;

    }
}