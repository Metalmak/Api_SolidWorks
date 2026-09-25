<!-- source: sldworksapi/Get_and_Set_State_of_Flyout_FeatureManager_Design_Tree_Example_VB.htm -->

# SOLIDWORKS API Help

# Get and Set the State of the Flyout FeatureManager Design Tree Example (VBA)

This example shows how to display, expand, and hide the flyout FeatureManager
design tree.

'----------------------------------------------------------------------------

' Preconditions:
' 1. Open a model document.
' 2. Open the Immediate window.
'
' Postconditions:
' 1. Click **OK** to close each of the three message boxes after examining
the
'    graphics area.
' 2. Examine the Immediate window.
'---------------------------------------------------------------------------
Option Explicit

Dim swApp As SldWorks.SldWorks
Dim Part As SldWorks.ModelDoc2
Dim ext As SldWorks.ModelDocExtension
Dim Status As Long

Sub main()

    Set swApp = Application.**SldWorks**

    Set Part = swApp.**ActiveDoc**
    Set ext = Part.**Extension**
    Status = ext.**FlyoutFeatureTreeVisibility**

    Debug.Print "-------Flyout state at
start-------"
    If Status = swFlyoutFeatureTree\_Hidden Then Debug.Print "FlyoutFeatureTree
Hidden"
    If Status = swFlyoutFeatureTree\_ShownExpanded Then
Debug.Print "FlyoutFeatureTree Expanded"
    If Status = swFlyoutFeatureTree\_ShownUnExpanded Then
Debug.Print "FlyoutFeatureTree UnExpanded"

    ext.**FlyoutFeatureTreeVisibility** =
swFlyoutFeatureTree\_ShownExpanded
    Status = ext.**FlyoutFeatureTreeVisibility**
    If Status = swFlyoutFeatureTree\_ShownExpanded Then MsgBox ("Flyout
state is now swFlyoutFeatureTree\_ShownExpanded.")

    ext.**FlyoutFeatureTreeVisibility** =
swFlyoutFeatureTree\_ShownUnExpanded
    Status = ext.**FlyoutFeatureTreeVisibility**
    If Status = swFlyoutFeatureTree\_ShownUnExpanded Then MsgBox
("Flyout state is now swFlyoutFeatureTree\_ShownUnExpanded.")

    ext.**FlyoutFeatureTreeVisibility** =
swFlyoutFeatureTree\_Hidden
    Status = ext.**FlyoutFeatureTreeVisibility**
    If Status = swFlyoutFeatureTree\_Hidden Then MsgBox ("Flyout
state is now swFlyoutFeatureTree\_Hidden.")

End Sub