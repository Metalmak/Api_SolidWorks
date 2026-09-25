<!-- source: sldworksapi/Add_Task_Pane_View_Example_VB.htm -->

# SOLIDWORKS API Help

# Add Task Pane View Example (VBA)

This example shows how to add a tab to the Task Pane.

'---------------------------------------------------------------------------
' Preconditions:
' 1. Create bitmaps in 6 pixel sizes:
'
20 X 20
'    32 X 32
'    40 X 40
'
64 X 64
'    96 X 96
'    128 X 128
' 2.
Replace the bitmap array elements in the macro to full pathnames of
'
these bitmap files.
'
' Postconditions:
' 1. Examine the Task Pane.
' 2. Displays a tab on the Task Pane with an
image that is appropriate for
'    the current screen
resolution or operating system scale.
'---------------------------------------------------------------------------

Option Explicit

Dim swApp As SldWorks.SldWorks
Dim ctrl As SldWorks.TaskpaneView
Dim bitmap(5) As String
Dim toolTip As String

Sub main()

     Set swApp = Application.SldWorks

     bitmap(0) =
"20x20\_bitmap\_pathname"

     bitmap(1) = "32x32\_bitmap\_pathname"

     bitmap(2) = "40x40\_bitmap\_pathname"

     bitmap(3) = "64x64\_bitmap\_pathname"

     bitmap(4) = "96x96\_bitmap\_pathname"

     bitmap(5) =
"128x128\_bitmap\_pathname"

    toolTip = ""
    Set ctrl = swApp.**CreateTaskpaneView3**(bitmap, toolTip)

End Sub