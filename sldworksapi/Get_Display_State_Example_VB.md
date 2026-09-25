<!-- source: sldworksapi/Get_Display_State_Example_VB.htm -->

# SOLIDWORKS API Help

# Get Display State Example (VBA)

This example shows how to get the display state of the model.

'-------------------------------------------

'

' Preconditions: Model document is open.

'

' Postconditions: None

'

'-------------------------------------------

Option Explicit

Public Enum swViewDisplayType\_e

    swIsViewSectioned
= 0

    swIsViewPerspective
= 1

    swIsViewShaded
= 2

    swIsViewWireFrame
= 3

    swIsViewHiddenLinesRemoved
= 4

    swIsViewHiddenInGrey
= 5

    swIsViewCurvature
= 6

End Enum

Sub main()

    Dim
swApp                       As
SldWorks.SldWorks

    Dim
swModel                     As
SldWorks.ModelDoc2

    Dim
swModView                   As
SldWorks.ModelView

    Set
swApp = Application.SldWorks

    Set
swModel = swApp.ActiveDoc

    Set
swModView = swModel.ActiveView

    Debug.Print
"File = " & swModel.GetPathName

    Debug.Print
"  Sectioned
           =
" & swModView.GetDisplayState(swIsViewSectioned)

    Debug.Print
"  Perspective
         =
" & swModView.GetDisplayState(swIsViewPerspective)

    Debug.Print
"  Shaded
              =
" & swModView.GetDisplayState(swIsViewShaded)

    Debug.Print
"  WireFrame
           =
" & swModView.GetDisplayState(swIsViewWireFrame)

    Debug.Print
"  HiddenLinesRemoved
  =
" & swModView.GetDisplayState(swIsViewHiddenLinesRemoved)

    Debug.Print
"  HiddenInGrey
        =
" & swModView.GetDisplayState(swIsViewHiddenInGrey)

    Debug.Print
"  Curvature
           =
" & swModView.GetDisplayState(swIsViewCurvature)

End Sub

'-------------------------------------------