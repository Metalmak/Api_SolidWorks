<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2~OnStringValueChanged.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnStringValueChanged Method (ISwManipulatorHandler2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwManipulatorHandler2 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2.html) : OnStringValueChanged Method (ISwManipulatorHandler2) |

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
:   ID of the string value to change

*Value*
:   New string value

Indicates if the new value for the specified item is accepted or not.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function OnStringValueChanged( _    ByVal pManipulator As System.Object, _    ByVal handleIndex As System.Integer, _    ByRef Value As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwManipulatorHandler2 Dim pManipulator As System.Object Dim handleIndex As System.Integer Dim Value As System.String Dim value As System.Boolean   value = instance.OnStringValueChanged(pManipulator, handleIndex, Value) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool OnStringValueChanged(     System.object pManipulator,    System.int handleIndex,    ref System.string Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool OnStringValueChanged(  &   System.Object^ pManipulator, &   System.int handleIndex, &   System.String^% Value ) ``` | |

#### Parameters

*pManipulator*
:   IManipulator object

*handleIndex*
:   ID of the string value to change

*Value*
:   New string value

#### Return Value

True if the add-in application accepts the new string value, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwManipulatorHandler2::OnStringValueChanged.

# ![](dotnetimages/collapse.gif)Example

See the [ISwManipulatorHandler2](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwManipulatorHandler2 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2.html)

[ISwManipulatorHandler2 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0