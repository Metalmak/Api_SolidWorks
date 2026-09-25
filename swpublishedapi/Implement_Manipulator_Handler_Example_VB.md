<!-- source: swpublishedapi/Implement_Manipulator_Handler_Example_VB.htm -->

# SOLIDWORKS API Help

# Implement Manipulator Handler Example (VBA)

This example shows how to implement a manipulator handler.

'-----------------------------------------------------------------------------

Option Explicit

Implements SwManipulatorHandler2

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Private Function SwManipulatorHandler2\_OnDelete(ByVal
pManipulator As Object) As Boolean

    Debug.Print
"SwManipulatorHandler2\_OnDelete"

End Function

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Private Sub SwManipulatorHandler2\_OnDirectionFlipped(ByVal
pManipulator As Object)

    Debug.Assert
False

    Debug.Print
"SwManipulatorHandler2\_OnDirectionFlipped"

End Sub

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Private Function SwManipulatorHandler2\_OnDoubleValueChanged(ByVal
pManipulator As Object, ByVal Id As Long, Value As Double) As Boolean

    'Debug.Assert
False

    Debug.Print
"SwManipulatorHandler2\_OnDoubleValueChanged"

    Debug.Print
"  ID
              =
" & Id

    Debug.Print
"  Value
           =
" & Value

End Function

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Private Sub SwManipulatorHandler2\_OnEndDrag(ByVal
pManipulator As Object)

    Debug.Print
"SwManipulatorHandler2\_OnEndDrag"

End Sub

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Private Sub SwManipulatorHandler2\_OnEndDrag(ByVal
pManipulator As Object, ByVal handleIndex As Long)

    Debug.Print
"SwManipulatorHandler2\_OnEndDrag"

    Debug.Print
"  HandleIndex
     =
" & handleIndex

    If
(handleIndex = swDragArrowManipulatorOptions\_e.swDragArrowManipulatorDirection2)
Then

        Debug.Print
" Direction1"

    Else

        Debug.Print
" Direction2"

    End
If

End Sub

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Private Sub SwManipulatorHandler2\_OnHandleRmbSelected(ByVal
pManipulator As Object, ByVal handleIndex As Long)

    Debug.Print
"SwManipulatorHandler2\_OnHandleRmbSelected"

    Debug.Print
"  handleIndex
     =
" + handleIndex

End Sub

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Private Sub SwManipulatorHandler2\_OnHandleSelected(ByVal
pManipulator As Object, ByVal handleIndex As Long)

    Debug.Print
"SwManipulatorHandler2\_OnHandleSelected"

    Debug.Print
"  HandleIndex
     =
" + handleIndex

End Sub

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Private Sub SwManipulatorHandler2\_OnItemSetFocus(ByVal
pManipulator As Object, ByVal Id As Long)

    Debug.Assert
False

    Debug.Print
"SwManipulatorHandler2\_OnItemSetFocus"

    Debug.Print
"  ID
              =
" & Id

End Sub

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Private Function SwManipulatorHandler2\_OnLmbSelected(ByVal
pManipulator As Object) As Boolean

    Debug.Assert
False

    Debug.Print
"SwManipulatorHandler2\_OnLmbSelected"

End Function

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Private Function SwManipulatorHandler2\_OnStringValueChanged(ByVal
pManipulator As Object, ByVal Id As Long, Value As String) As Boolean

    Debug.Assert
False

    Debug.Print
"SwManipulatorHandler2\_OnStringValueChanged"

    Debug.Print
"  ID
              =
" & Id

    Debug.Print
"  Value
           =
" & Value

End Function

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Private Sub SwManipulatorHandler2\_OnUpdateDrag(ByVal
pManipulator As Object, ByVal handleIndex As Long, ByVal newPosMathPt
As Object)

    Debug.Print
"SwManipulatorHandler2\_OnUpdateDrag"

    Debug.Print
"  HandleIndex
     =
" & handleIndex

End Sub