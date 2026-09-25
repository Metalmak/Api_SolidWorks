<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop2~Select.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Select Method (ILoop2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILoop2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop2.html) : Select Method (ILoop2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Edge*
:   [Edge](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) of the loop (see **Remarks**)

*Append*
:   True to append this selection to the selection list, false to replace the selection list with this selection

*SelectionData*
:   [ISelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData.html) object

Selects a loop in the graphics area.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Select( _    ByVal Edge As System.Object, _    ByVal Append As System.Boolean, _    ByVal SelectionData As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILoop2 Dim Edge As System.Object Dim Append As System.Boolean Dim SelectionData As System.Object Dim value As System.Boolean   value = instance.Select(Edge, Append, SelectionData) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Select(     System.object Edge,    System.bool Append,    System.object SelectionData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Select(  &   System.Object^ Edge, &   System.bool Append, &   System.Object^ SelectionData ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Edge*
:   [Edge](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) of the loop (see **Remarks**)

*Append*
:   True to append this selection to the selection list, false to replace the selection list with this selection

*SelectionData*
:   [ISelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData.html) object

#### Return Value

True if the loop is selected, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Loop2::Select.

# ![](dotnetimages/collapse.gif)Example

'VBA

'============================================

' Preconditions:

' 1. Open a model with a triangular face.

' 2. Multi-select the triangular face and one of its edges.

' 3. Comment out one of the highlighted lines with **swLoop.Select**.

' 4. Run the macro.

' 5. Comment out the other highlighted line.

' 6. Run the macro again.

' Postconditions:

' 1. Inspect the Immediate window after each run.

' 2. Notice that a different loop is selected each time.

'============================================

Option Explicit

Sub main()
    Dim swApp As SldWorks.SldWorks
    Set swApp = Application.SldWorks

    Dim swModel As ModelDoc2
    Set swModel = swApp.ActiveDoc
    If swModel Is Nothing Then Exit Sub

    Dim swSelMgr As SelectionMgr
    Set swSelMgr = swModel.SelectionManager

    Dim swFace As Face2
    Dim swEdge As Edge

    Dim iSel As Long
    For iSel = 1 To 2
        Select Case swSelMgr.GetSelectedObjectType3(iSel, -1)
        Case swSelFACES
            Set swFace = swSelMgr.GetSelectedObject6(iSel, -1)
        Case swSelEDGES
            Set swEdge = swSelMgr.GetSelectedObject6(iSel, -1)
        End Select
    Next

    If swFace Is Nothing Or swEdge Is Nothing Then Exit Sub

    Dim vLoops As Variant
    vLoops = swFace.**GetLoops**()

    Dim vLoop As Variant
    Dim swLoop As Loop2
    For Each vLoop In vLoops
        Set swLoop = vLoop
        Dim vEdges As Variant
        vEdges = swLoop.**GetEdges**()

        Dim loopUsesEdges As Boolean
        loopUsesEdges = False
        Dim vEdge As Variant
        For Each vEdge In vEdges
            If vEdge Is swEdge Then
                loopUsesEdges = True
                Exit For
            End If
        Next
        If loopUsesEdges Then
            ' Demonstrate that we have the right loop..
            Debug.Assert swLoop.**GetFace** Is swFace
            swModel.ClearSelection2 True
            For Each vEdge In vEdges
                Dim swLoopEdge As Entity
                Set swLoopEdge = vEdge
                swLoopEdge.Select4 True, Nothing
            Next
            Exit For
        Else
            Set swLoop = Nothing
        End If
    Next

    Stop ' Examine highlighted edges of this loop

    If Not swLoop Is Nothing Then
        Debug.Print "Loop has " & swLoop.**GetEdgeCount**() & " edges."

        Dim bResult As Boolean

**' Comment and uncomment out different lines after each run:** **bResult = swLoop.Select(swEdge, False, Nothing) 'Selects the adjacent loop
        'bResult = swLoop.Select(Nothing, False, Nothing) 'Selects this loop**
        Stop ' Examine highlighted edges of selected loop. This loop or its adjacent loop?

        Dim swSelLoop As Loop2
        Set swSelLoop = swSelMgr.**GetSelectedObjectLoop2**(1, -1)

        Debug.Print "Selected loop has " & swSelLoop.**GetEdgeCount**() & " edges."

        swModel.ClearSelection2 True
        vEdge = vbEmpty
        vEdge = swSelLoop.**GetEdges**()

        For Each vEdge In vEdges

            Set swLoopEdge = vEdge
            swLoopEdge.Select4 True, Nothing
        Next
        Debug.Print "Selected " & swSelMgr.GetSelectedObjectCount2(-1) & " edges in loop."
    End If

End Sub

# ![](dotnetimages/collapse.gif)Remarks

This loop can share Edge with an adjacent loop, if it exists.

If Edge is:

* a valid edge on this loop, this method selects the adjacent loop.* Nothing or null, this method selects this loop.

# ![](dotnetimages/collapse.gif)See Also

####

[ILoop2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop2.html)

[ILoop2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop2_members.html)

[DPartDocEvents\_FlipLoopNotifyEventHandler Delegate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_FlipLoopNotifyEventHandler.html)

[DAssemblyDocEvents\_FileDropNotifyEventHandler Delegate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_FileDropNotifyEventHandler.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0