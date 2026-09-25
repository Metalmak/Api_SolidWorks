<!-- source: sldworksapi/Show_Named_View_Example_VB.htm -->

# SOLIDWORKS API Help

# Show Named View Example (VBA)

This example shows how to get the name of a named view in an open model
document.

'--------------------------------------

'

' Preconditions: Model document is open.

'

' Postconditions: None

'

'---------------------------------------

Option Explicit

Dim swApp As SldWorks.SldWorks

Sub main()

    Dim
swModel      As
SldWorks.ModelDoc2

    Dim
lIdx         As
Long

    Dim
vTransform   As
Variant

    Set
swApp = Application.SldWorks

    Set
swModel = swApp.ActiveDoc

    For
lIdx = swStandardViews\_e.swFrontView To swStandardViews\_e.swDimetricView

        Debug.Print
"View = " & PrintViewName(lIdx) & " (" &
lIdx & ")"

        vTransform
= swModel.GetStandardViewRotation(lIdx)

        swModel.ShowNamedView2 "", lIdx

        Stop

    Next
lIdx

End Sub

Private Function PrintViewName(ByVal nView As swStandardViews\_e)
As String

    PrintViewName
= "<not a standard view>"

    Select
Case (nView)

        Case
swStandardViews\_e.swBackView

            PrintViewName
= "Back"

        Case
swStandardViews\_e.swBottomView

            PrintViewName
= "Bottom"

        Case
swStandardViews\_e.swDimetricView

            PrintViewName
= "Dimetric"

        Case
swStandardViews\_e.swFrontView

            PrintViewName
= "Front"

        Case
swStandardViews\_e.swIsometricView

            PrintViewName
= "Isometric"

        Case
swStandardViews\_e.swLeftView

            PrintViewName
= "Left"

        Case
swStandardViews\_e.swRightView

            PrintViewName
= "Right"

        Case
swStandardViews\_e.swTopView

            PrintViewName
= "Top"

        Case
swStandardViews\_e.swTrimetricView

            PrintViewName
= "Trimetric"

    End
Select

End Function