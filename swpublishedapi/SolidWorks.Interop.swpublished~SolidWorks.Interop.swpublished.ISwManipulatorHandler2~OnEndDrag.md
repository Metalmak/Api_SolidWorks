<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2~OnEndDrag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnEndDrag Method (ISwManipulatorHandler2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwManipulatorHandler2 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2.html) : OnEndDrag Method (ISwManipulatorHandler2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pManipulator*
:   IManipulator object

*handleIndex*
:   | If the manipulator is a... | Then use... |
    | --- | --- |
    | Drag arrow | swDragArrowManipulatorOptions\_e |
    | Triad | swTriadManipulatorControlPoints\_e |

Called when a user releases a mouse button after dragging the pointer.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnEndDrag( _    ByVal pManipulator As System.Object, _    ByVal handleIndex As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwManipulatorHandler2 Dim pManipulator As System.Object Dim handleIndex As System.Integer   instance.OnEndDrag(pManipulator, handleIndex) ``` | |

| C# |  |
| --- | --- |
| ``` void OnEndDrag(     System.object pManipulator,    System.int handleIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnEndDrag(  &   System.Object^ pManipulator, &   System.int handleIndex ) ``` | |

#### Parameters

*pManipulator*
:   IManipulator object

*handleIndex*
:   | If the manipulator is a... | Then use... |
    | --- | --- |
    | Drag arrow | swDragArrowManipulatorOptions\_e |
    | Triad | swTriadManipulatorControlPoints\_e |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwManipulatorHandler2::OnEndDrag.

# ![](dotnetimages/collapse.gif)Example

See the [ISwManipulatorHandler2](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwManipulatorHandler2 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2.html)

[ISwManipulatorHandler2 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2_members.html)

[IswManipulatorHandler2::OnEndNoDrag Method ()](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2~OnEndNoDrag.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0