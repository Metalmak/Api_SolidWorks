<!-- source: sldworksapi/Position_a_Document_Window_Example_VB.htm -->

# SOLIDWORKS API Help

# Position Document Window Example (VBA)

This example shows how to position the current
document window.

'---------------------------------------------

' Assumes part is already set to a IModelDoc2
object

' Get the IModelView object

Set ModelView = Part.ActiveView

' Position the window

ModelView.FrameLeft
= 100

ModelView.FrameWidth
= 500

ModelView.FrameTop
= 100

ModelView.FrameHeight
= 400

ModelView.FrameState
= swWindowNormal