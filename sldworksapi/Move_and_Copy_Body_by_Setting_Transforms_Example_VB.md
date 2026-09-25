<!-- source: sldworksapi/Move_and_Copy_Body_by_Setting_Transforms_Example_VB.htm -->

# SOLIDWORKS API Help

# Move and Copy Body by Setting Transforms Example (VBA)

This example shows how to move and copy bodies by setting transforms.

'----------------------------------------------------------

'

' Preconditions:

'    (1)
Part document is open.

'    (2)
Body-Move/Copy1 feature exists.

'

' Postconditions: Body is moved and copied as per transform
settings.

'

'-----------------------------------------------------------

Option Explicit

Sub main()

    Dim
swApp As SldWorks.SldWorks

    Dim
part As SldWorks.PartDoc

    Dim
component As SldWorks.Component2

    Dim
moveCopyFeat As SldWorks.feature

    Dim
moveCopy\_featData As SldWorks.MoveCopyBodyFeatureData

    Dim
boolstatus As Boolean

    Set
swApp = Application.SldWorks

    Set
part = swApp.ActiveDoc

    Set
moveCopyFeat = part.FeatureByName("Body-Move/Copy1")

    Set
moveCopy\_featData = moveCopyFeat.GetDefinition

    boolstatus
= moveCopy\_featData.AccessSelections(part,
component)

    moveCopy\_featData.TransformType = swTransformType\_Translation

    moveCopy\_featData.TransformX = 0.02

    moveCopy\_featData.TransformY = 0.03

    moveCopy\_featData.TransformZ = 0.04

    boolstatus
= moveCopyFeat.ModifyDefinition(moveCopy\_featData,
part, Nothing)

    moveCopy\_featData.ReleaseSelectionAccess

End Sub