<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler~OnUpdateDrag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnUpdateDrag Method (ISwManipulatorHandler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwManipulatorHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler.html) : OnUpdateDrag Method (ISwManipulatorHandler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pManipulator*

*handleIndex*

*newPosMathPt*

Obsolete. Superseded by [ISwManipulatorHandler2::OnUpdateDrag](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.ISwManipulatorHandler2~OnUpdateDrag.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnUpdateDrag( _    ByVal pManipulator As System.Object, _    ByVal handleIndex As System.Integer, _    ByVal newPosMathPt As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwManipulatorHandler Dim pManipulator As System.Object Dim handleIndex As System.Integer Dim newPosMathPt As System.Object   instance.OnUpdateDrag(pManipulator, handleIndex, newPosMathPt) ``` | |

| C# |  |
| --- | --- |
| ``` void OnUpdateDrag(     System.object pManipulator,    System.int handleIndex,    System.object newPosMathPt ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnUpdateDrag(  &   System.Object^ pManipulator, &   System.int handleIndex, &   System.Object^ newPosMathPt ) ``` | |

#### Parameters

*pManipulator*

*handleIndex*

*newPosMathPt*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwManipulatorHandler::OnUpdateDrag.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwManipulatorHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler.html)

[ISwManipulatorHandler Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler_members.html)