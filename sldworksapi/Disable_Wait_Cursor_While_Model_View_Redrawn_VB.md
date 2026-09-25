<!-- source: sldworksapi/Disable_Wait_Cursor_While_Model_View_Redrawn_VB.htm -->

# SOLIDWORKS API Help

# Disable Wait Cursor When Model View Redrawn (VBA)

This example shows how to suppress the wait cursor (also called the
hourglass) when a model view is redrawn.

'---------------------------------------------

Option Explicit

Sub main()

    Dim
swApp As Object

    Dim
Part As SldWorks.ModelDoc2

    Dim
modelView As SldWorks.modelView

    Set
swApp = Application.SldWorks

    Set
Part = swApp.ActiveDoc

    Set
modelView = Part.ActiveView

    modelView.SuppressWaitCursorDuringRedraw = False

End Sub