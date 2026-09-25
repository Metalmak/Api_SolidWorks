<!-- source: sldworksapi/Change_to_Isometric_and_Zoom_to_Fit_View_Mode_Example_VB.htm -->

# SOLIDWORKS API Help

# Change to Isometric and Zoom to Fit View Mode Example (VBA)

This example shows how to change the current view mode to isometric
and Zoom to Fit.

'-----------------------------------------------

'

' Preconditions: Model document is open.

'

' Postconditions: Current view mode is changed to isometric
and Zoom to Fit.

'

'-----------------------------------------------

Option Explicit

Sub main()

    Dim
swApp                   As
SldWorks.SldWorks

    Dim
swModel                 As
SldWorks.ModelDoc2

    Set
swApp = CreateObject("SldWorks.Application")

    Set
swModel = swApp.ActiveDoc

    '
Not quite the same as when done through the user interface;

    '
model is zoomed out a bit further

    swModel.ShowNamedView2 "\*Isometric",
-1

    '
Now view the same as done through the user interface

    swModel.ViewZoomtofit2

End Sub

'-----------------------------------------------