<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler~OnDoubleValueChanged.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnDoubleValueChanged Method (ISwManipulatorHandler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwManipulatorHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler.html) : OnDoubleValueChanged Method (ISwManipulatorHandler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pManipulator*

*Id*

*Value*

Obsolete. Superseded by [ISwManipulatorHandler2::OnDoubleValueChanged](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.ISwManipulatorHandler2~OnDoubleValueChanged.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function OnDoubleValueChanged( _    ByVal pManipulator As System.Object, _    ByVal Id As System.Integer, _    ByRef Value As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwManipulatorHandler Dim pManipulator As System.Object Dim Id As System.Integer Dim Value As System.Double Dim value As System.Boolean   value = instance.OnDoubleValueChanged(pManipulator, Id, Value) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool OnDoubleValueChanged(     System.object pManipulator,    System.int Id,    ref System.double Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool OnDoubleValueChanged(  &   System.Object^ pManipulator, &   System.int Id, &   System.double% Value ) ``` | |

#### Parameters

*pManipulator*

*Id*

*Value*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwManipulatorHandler::OnDoubleValueChanged.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwManipulatorHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler.html)

[ISwManipulatorHandler Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler_members.html)