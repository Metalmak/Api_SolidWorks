<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2~OnHandleSelected.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnHandleSelected Method (ISwManipulatorHandler2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwManipulatorHandler2 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2.html) : OnHandleSelected Method (ISwManipulatorHandler2) |

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
:   Direction of the drag handle as defined by swDragArrowManipulatorOptions\_e

Gets the selected handle for this manipulator.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnHandleSelected( _    ByVal pManipulator As System.Object, _    ByVal handleIndex As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwManipulatorHandler2 Dim pManipulator As System.Object Dim handleIndex As System.Integer   instance.OnHandleSelected(pManipulator, handleIndex) ``` | |

| C# |  |
| --- | --- |
| ``` void OnHandleSelected(     System.object pManipulator,    System.int handleIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnHandleSelected(  &   System.Object^ pManipulator, &   System.int handleIndex ) ``` | |

#### Parameters

*pManipulator*
:   IManipulator object

*handleIndex*
:   Direction of the drag handle as defined by swDragArrowManipulatorOptions\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwManipulatorHandler2::OnHandleSelected.

# ![](dotnetimages/collapse.gif)Example

See the [ISwManipulatorHandler2](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwManipulatorHandler2 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2.html)

[ISwManipulatorHandler2 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0