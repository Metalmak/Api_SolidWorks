<!-- source: sldworksapi/Create_and_Arrange_Windows_Example_VB.htm -->

# SOLIDWORKS API Help

# Create and Arrange Windows Example (VBA)

This example shows how to create a new window containing the active
document object and how to arrange all open windows.

'-------------------------------------

Option Explicit

Sub main()

    Dim
swApp As SldWorks.SldWorks

    Set
swApp = Application.SldWorks

    swApp.CreateNewWindow

    '
  Arrange:

'   0
= Cascade

    '
  1
= Tile horizontally

    '
  2
= Tile vertically

    swApp.ArrangeWindows 1

End Sub

'-------------------------------------