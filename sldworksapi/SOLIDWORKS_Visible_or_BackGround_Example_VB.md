<!-- source: sldworksapi/SOLIDWORKS_Visible_or_BackGround_Example_VB.htm -->

# SOLIDWORKS API Help

# SOLIDWORKS Visible or Background Example (VBA)

These examples shows several situations for
running or attaching to SOLIDWORKS session through the API.

## SOLIDWORKS not running: Launch invisibly and end SOLIDWORKS session

Sub Macro1()

     Dim
swApp As Object

     Set
swApp = CreateObject("SldWorks.Application")

     ' Close
the SOLIDWORKS application. If you do not perform this step, SOLIDWORKS

' continues to run. If SOLIDWORKS is running in the background, the user
is

' unaware that SOLIDWORKS is running and consuming their system resources.

     swApp.ExitApp

     Set
swApp = Nothing

End Sub

## SOLIDWORKS running: Attach to existing SOLIDWORKS session and end SOLIDWORKS session

Sub Macro2()

     Dim
swApp As Object

     Set
swApp = CreateObject("SldWorks.Application")

     swApp.ExitApp

     Set
swApp = Nothing

End Sub

## SOLIDWORKS not running: Launch invisibly, become visible, and end SOLIDWORKS session

Sub Macro3()

     Dim
swApp As Object

     Dim
Part As Object

     Set
swApp = CreateObject("SldWorks.Application")

     swApp.Visible = True

     swApp.ExitApp

     Set
swApp = Nothing

End Sub

## SOLIDWORKS not running: Launch invisibly, become visible, and leave SOLIDWORKS running

Sub Macro4()

     Dim
swApp As Object

     Set
swApp = CreateObject("SldWorks.Application")

     swApp.Visible = True

     swApp.UserControl = True

     '
Give control to the user, which leaves SOLIDWORKS running

End Sub

## SOLIDWORKS not running: Launch invisibly, create part invisibly, close part, and end SOLIDWORKS session

Sub Macro5()

     Dim
swApp As Object

     Dim
Part As Object

     '
This must be explicitly defined for ISldWorks::ActivateDoc2

     Dim
errors As Long

     Set
swApp = CreateObject("SldWorks.Application")

     Set
Part = swApp.NewPart

     Set
Part = swApp.ActivateDoc2("Part1",True,errors)

     Set
Part = Nothing

     swApp.CloseDoc "Part1"

     swApp.ExitApp

Set
swApp = Nothing

End Sub

## SOLIDWORKS not running: Launch invisibly, create part invisibly, make the part and SOLIDWORKS visible, and leave SOLIDWORKS running

Sub Macro6()

     Dim
swApp As Object

     Dim
Part As Object

     Set
swApp = CreateObject("SldWorks.Application")

     Set
Part = swApp.NewPart

     Set
Part = swApp.ActivateDoc("Part1")

     Part.Visible = True

     '
Make the part and SOLIDWORKS visible

     swApp.UserControl = True

     '
Give control to the user, which leaves SOLIDWORKS running

     Set
Part = Nothing

     swApp.CloseDoc "Part1"

End Sub