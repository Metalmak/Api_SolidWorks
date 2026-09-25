<!-- source: swpublishedapi/Create_Triad_Manipulator_Example_VB.htm -->

# SOLIDWORKS API Help

# Create Triad Manipulator Example (VBA)

This example shows how to create a triad manipulator.

'----------------------------------------------------------------------------
' Preconditions:
' 1. Click **Tools > References** **>** **SolidWorks 2015 exposed type libraries
for
'    add-in use** (**swpublished.tlb**) and click **OK**.
' 2. Right-click the project name in the Project Explorer and
click
'    **Insert > Class Module**.
' 3. Click **Class1** in the Project Explorer.
' 4. Type **swDragManipHdlr** in **(Name)** in the Properties
window.
' 5. Copy [Module](#Module) to the main module.
' 6. Copy [Class
module](#Class) to the swDragManipHdlr class module.
' 7. Open a model document and select a face.
' 8. Open an Immediate window.
'
' Postconditions:
' 1. Creates a triad manipulator whose origin is the point
'    selected on the face.
' 2. Drag a triad manipulator handle and inspect the Immediate window.
'----------------------------------------------------------------------------

### 'Module

Option Explicit

Dim
swManip                  As
SldWorks.Manipulator

Dim swTriad                  As
SldWorks.TriadManipulator

Dim
swDragHdlr               As
swDragManipHdlr

Dim swFace                   As
SldWorks.Face2

Sub main()

    Dim
swApp                       As
SldWorks.SldWorks

    Dim
swMathUtil                  As
SldWorks.MathUtility

    Dim
swModel                     As
SldWorks.ModelDoc2

    Dim
swModViewMgr                As
SldWorks.ModelViewManager

    Dim
swSelMgr                    As
SldWorks.SelectionMgr

    Dim
vPickPt                     As
Variant

    Dim
swPickPt                    As
SldWorks.MathPoint

    Set
swDragHdlr = New swDragManipHdlr

    Set
swApp = Application.SldWorks

    Set
swMathUtil = swApp.GetMathUtility

    Set
swModel = swApp.ActiveDoc

    Set
swSelMgr = swModel.SelectionManager

    Set
swFace = swSelMgr.GetSelectedObject6(1,
-1)

    vPickPt
= swSelMgr.GetSelectionPoint2(1, -1)

    Set
swPickPt = swMathUtil.CreatePoint((vPickPt))

    Set
swModViewMgr = swModel.ModelViewManager

    Set
swManip = swModViewMgr.CreateManipulator(swTriadManipulator,
swDragHdlr)

    Set
swTriad = swManip.GetSpecificManipulator

    swTriad.Origin = swPickPt

    swManip.Show swModel

End Sub

[Back to top](#top)

### 'Class module

Option Explicit

Implements SwManipulatorHandler2

Private Function SwManipulatorHandler2\_OnDelete(ByVal
pManipulator As Object) As Boolean

    Debug.Print
"Manipulator deleted"

End Function

Private Sub SwManipulatorHandler2\_OnDirectionFlipped(ByVal
pManipulator As Object)

    Debug.Print
"Direction flipped"

End Sub

Private Function
SwManipulatorHandler2\_OnDoubleValueChanged(ByVal pManipulator As Object, ByVal
Id As Long, Value As Double) As Boolean

    Debug.Print
"Double value changed "

    Debug.Print "  Value
= " & Value

End Function

Private Sub SwManipulatorHandler2\_OnEndNoDrag(ByVal
pManipulator As Object, ByVal handleIndex As Long)

    Debug.Print "Mouse button released"

    Debug.Print "  HandleIndex  as
defined in swTriadManipulatorControlPoints\_e
= " + handleIndex

End Sub

Private Sub SwManipulatorHandler2\_OnEndDrag(ByVal
pManipulator As Object, ByVal handleIndex As Long)

    Debug.Print
"Mouse button released after dragging a manipulator handle"

End Sub

Private Sub SwManipulatorHandler2\_OnHandleRmbSelected(ByVal
pManipulator As Object, ByVal handleIndex As Long)

    Debug.Print
"Right-mouse button clicked"

    Debug.Print "  HandleIndex as
defined in swTriadManipulatorControlPoints\_e
= " + handleIndex

End Sub

Private Sub SwManipulatorHandler2\_OnHandleSelected(ByVal
pManipulator As Object, ByVal handleIndex As Long)

    Debug.Print "Manipulator handle selected"

    Debug.Print "  HandleIndex
= " + handleIndex

End Sub

Private Sub SwManipulatorHandler2\_OnItemSetFocus(ByVal
pManipulator As Object, ByVal Id As Long)

    Debug.Print
"Focus set on item"

    Debug.Print "  Item ID
= " & Id

End Sub

Private Function
SwManipulatorHandler2\_OnHandleLmbSelected(ByVal pManipulator As Object) As
Boolean

    Debug.Print
"Left-mouse button clicked"

End Function

Private Function
SwManipulatorHandler2\_OnStringValueChanged(ByVal pManipulator As Object, ByVal
Id As Long, Value As String) As Boolean

    Debug.Print
"String value changed"

    Debug.Print "  Value
= " & Value

End Function

Private Sub SwManipulatorHandler2\_OnUpdateDrag(ByVal
pManipulator As Object, ByVal handleIndex As Long, ByVal newPosMathPt As Object)

    Debug.Print
"Manipulator handle moved while left- or right-mouse button depressed"

    Debug.Print "  HandleIndex as
defined in swTriadManipulatorControlPoints\_e
= " & handleIndex

End Sub

[Back to top](#top)