<!-- source: sldworksapi/Edit_Balloon_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Edit Balloon Example (VB.NET)

This example shows how to edit a balloon in a drawing document.

'
--------------------------------------------------------------------------
' Preconditions:
' 1. Open *public\_documents***\samples\tutorial\advdrawings\foodprocessor.slddrw.**
' 2. Click **Insert > Annotations > Balloon**.
' 3. Click a model edge in either drawing view and add the balloon.
' 4. Close the Balloon PropertyManager page.
' 5. Select the balloon in the drawing.
'
' Postconditions: The properties of the selected balloon are modified.
'
' **NOTE:** Because this drawing document is used elsewhere, do not save any
' changes when closing it.
' --------------------------------------------------------------------------
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
Class
SolidWorksMacro

    Dim
swModel As
ModelDoc2
    Dim
swModelDocExt As
ModelDocExtension
    Dim
swSelMgr As
SelectionMgr
    Dim
swNote As
Note

    Sub
main()

        swModel = swApp.**ActiveDoc**
        swModelDocExt = swModel.**Extension**
        swSelMgr = swModel.**SelectionManager**

        ' Get the selected balloon
        swNote = swSelMgr.**GetSelectedObject6**(1,
-1)

        ' Edit the selected balloon
        swNote = swModelDocExt.**EditBalloonProperties2**(swBalloonStyle\_e.swBS\_SplitCirc,
swBalloonFit\_e.swBF\_5Chars, swBalloonTextContent\_e.swBalloonTextCustom,
"Upper",
swBalloonTextContent\_e.swBalloonTextCustom,
"Lower", 0,
True, 1,
"X",
0.0355)

        Debug.Print("Balloon name:  "
& swNote.**GetName**)

    End
Sub

    Public
swApp As
SldWorks

End
Class