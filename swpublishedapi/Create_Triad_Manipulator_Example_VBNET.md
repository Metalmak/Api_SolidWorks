<!-- source: swpublishedapi/Create_Triad_Manipulator_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Create Triad Manipulator Example (VB.NET)

This example shows how to create a triad manipulator.

'----------------------------------------------------------------------------
' Preconditions:

' 1. Right-click the project name in the Project Explorer and click
'    **Add Reference**.
' 2. On the Browse tab, navigate to *install\_dir***\api\redist**,
click
'    **SolidWorks.Interop.swpublished.dll,** and click **OK**.

' 3. Right-click the project name in the Project Explorer and click
'    **Add > Class**.
' 4. Type **swDragManipHdlr.vb** in **Name** and click **Add**.
' 5. Copy [Module](#Module) to **SolidWorksMacro.vb**.
' 6. Copy [Class module](#Class module) to **swDragManipHdlr.vb**.
' 7. Click **Tools > Options** and ensure that **Stop VSTA debugger on macro exit**
'    is not selected.
' 8. Open a model document and select a face.
' 9. Open an Immediate window.
'
' Postconditions:

' 1. Creates a triad manipulator whose origin is the point
'    selected on the face.
' 2. Drag a triad manipulator handle
and inspect the Immediate window.

'----------------------------------------------------------------------------

'**Module**

Imports SolidWorks.Interop.sldworks
Imports SolidWorks.Interop.swconst
Imports System.Runtime.InteropServices
Imports System

Partial Class SolidWorksMacro

    Dim swDragHdlr As swDragManipHdlr

    Sub main()

        Dim swManip As Manipulator
        Dim swTriad As TriadManipulator
        Dim swFace As Face2
        Dim swMathUtil As MathUtility
        Dim swModel As ModelDoc2
        Dim swModViewMgr As ModelViewManager
        Dim swSelMgr As SelectionMgr
        Dim vPickPt As Object
        Dim swPickPt As MathPoint

        swDragHdlr = New swDragManipHdlr

        swMathUtil = swApp.**GetMathUtility**
        swModel = swApp.**ActiveDoc**
        swSelMgr = swModel.**SelectionManager**
        swFace = swSelMgr.**GetSelectedObject6**(1, -1)

        vPickPt = swSelMgr.**GetSelectionPoint2**(1, -1)
        swPickPt = swMathUtil.**CreatePoint**((vPickPt))
        swModViewMgr = swModel.**ModelViewManager**

        swManip = swModViewMgr.**CreateManipulator**(swManipulatorType\_e.swTriadManipulator, swDragHdlr)
        swTriad = swManip.**GetSpecificManipulator**
        swTriad.**Origin** = swPickPt
        swManip.**Show**(swModel)

    End Sub

    Public swApp As SldWorks

End Class

[Back to top](#top)

**'Class module**

Imports SolidWorks.Interop.swpublished
Imports SolidWorks.Interop.swconst
Imports System.Diagnostics

<System.Runtime.InteropServices.ComVisibleAttribute(True)> \_
Public Class swDragManipHdlr
    Implements SwManipulatorHandler2

    Private Function SwManipulatorHandler2\_OnDelete(ByVal pManipulator As Object) As Boolean Implements SwManipulatorHandler2.**OnDelete**
        Debug.Print("Manipulator deleted")
    End Function

    Private Sub SwManipulatorHandler2\_OnDirectionFlipped(ByVal pManipulator As Object) Implements SwManipulatorHandler2.**OnDirectionFlipped**
        Debug.Print("Direction flipped")
    End Sub

    Private Function SwManipulatorHandler2\_OnDoubleValueChanged(ByVal pManipulator As Object, ByVal handleIndex As Integer, ByRef Value As Double) As Boolean Implements SwManipulatorHandler2.**OnDoubleValueChanged**
        Debug.Print("Double value changed")
        Debug.Print("  Value = " & Value)
    End Function

    Private Sub SwManipulatorHandler2\_OnEndNoDrag(ByVal pManipulator As Object, ByVal handleIndex As Integer) Implements SwManipulatorHandler2.**OnEndNoDrag**
        Debug.Print("Mouse button released")
    End Sub

    Private Sub SwManipulatorHandler2\_OnEndDrag(ByVal pManipulator As Object, ByVal handleIndex As Integer) Implements SwManipulatorHandler2.**OnEndDrag**
        Debug.Print("Mouse
button released after dragging a manipulator handle")
    End Sub

    Private Sub SwManipulatorHandler2\_OnHandleRmbSelected(ByVal pManipulator As Object, ByVal handleIndex As Integer) Implements SwManipulatorHandler2.**OnHandleRmbSelected**
        Debug.Print("Right-mouse button clicked")
        Debug.Print("  HandleIndex = " + handleIndex)
    End Sub

    Private Sub SwManipulatorHandler2\_OnHandleSelected(ByVal pManipulator As Object, ByVal handleIndex As Integer) Implements SwManipulatorHandler2.**OnHandleSelected**
        Debug.Print("Manipulator handle selected")
        Debug.Print("  HandleIndex = " + handleIndex)
    End Sub

    Private Sub SwManipulatorHandler2\_OnItemSetFocus(ByVal pManipulator As Object, ByVal Id As Integer) Implements SwManipulatorHandler2.**OnItemSetFocus**
        Debug.Print("Focus set on item")
        Debug.Print("  Item ID = " & Id)
    End Sub

    Private Function SwManipulatorHandler2\_OnHandleLmbSelected(ByVal pManipulator As Object) As Boolean Implements SwManipulatorHandler2.**OnHandleLmbSelected**
        Debug.Print("Left-mouse button clicked")
    End Function

    Private Function SwManipulatorHandler2\_OnStringValueChanged(ByVal pManipulator As Object, ByVal handleIndex As Integer, ByRef Value As String) As Boolean Implements SwManipulatorHandler2.**OnStringValueChanged**
        Debug.Print("String value changed")
        Debug.Print("  String value  = " & Value)
    End Function

    Private Sub SwManipulatorHandler2\_OnUpdateDrag(ByVal pManipulator As Object, ByVal handleIndex As Integer, ByVal newPosMathPt As Object) Implements SwManipulatorHandler2.**OnUpdateDrag**
        Debug.Print("Manipulator handle moved while
left- or right-mouse button depressed")
        Debug.Print("  HandleIndex = " & handleIndex)
    End Sub

End Class

[Back to top](#top)