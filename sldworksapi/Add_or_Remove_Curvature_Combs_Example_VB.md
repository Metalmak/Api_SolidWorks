<!-- source: sldworksapi/Add_or_Remove_Curvature_Combs_Example_VB.htm -->

# SOLIDWORKS API Help

# Add or Remove Curvature Combs Example (VBA)

This example shows how to add or remove curvature combs to a curved
sketch segment.

'----------------------------------------------------

' Preconditions: Curved sketch segment is selected.

'

' Postconditions: Curvature combs are added or removed.

'----------------------------------------------------

Option Explicit

Sub main()

    Dim
swApp                   As
SldWorks.SldWorks

    Dim
swModel                 As
SldWorks.ModelDoc2

    Dim
nResponse               As
Integer

    Dim
bRet                    As
Boolean

    Set
swApp = Application.SldWorks

    Set
swModel = swApp.ActiveDoc

    nResponse
= MsgBox("Add curvature combs?", vbYesNo)

    If
nResponse = vbYes Then

        swModel.InspectCurvature

    Else

        swModel.RemoveInspectCurvature

    End
If

End Sub