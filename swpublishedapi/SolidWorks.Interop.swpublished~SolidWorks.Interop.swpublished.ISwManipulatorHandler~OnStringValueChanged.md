<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler~OnStringValueChanged.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnStringValueChanged Method (ISwManipulatorHandler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwManipulatorHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler.html) : OnStringValueChanged Method (ISwManipulatorHandler) |

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

Obsolete. Superseded by [ISwManipulatorHandler2::OnStringValueChanged](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.ISwManipulatorHandler2~OnStringValueChanged.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function OnStringValueChanged( _    ByVal pManipulator As System.Object, _    ByVal Id As System.Integer, _    ByRef Value As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwManipulatorHandler Dim pManipulator As System.Object Dim Id As System.Integer Dim Value As System.String Dim value As System.Boolean   value = instance.OnStringValueChanged(pManipulator, Id, Value) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool OnStringValueChanged(     System.object pManipulator,    System.int Id,    ref System.string Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool OnStringValueChanged(  &   System.Object^ pManipulator, &   System.int Id, &   System.String^% Value ) ``` | |

#### Parameters

*pManipulator*

*Id*

*Value*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwManipulatorHandler::OnStringValueChanged.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwManipulatorHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler.html)

[ISwManipulatorHandler Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler_members.html)