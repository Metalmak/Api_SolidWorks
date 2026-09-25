<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwCalloutHandler~OnStringValueChanged.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnStringValueChanged Method (ISwCalloutHandler) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwCalloutHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwCalloutHandler.html) : OnStringValueChanged Method (ISwCalloutHandler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pManipulator*
:   ICallout object whose text was edited

*RowID*
:   Row in which the text was edi

*Text*
:   New text of RowID

Allows access to and modifcation of text in a specific row in a callout.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function OnStringValueChanged( _    ByVal pManipulator As System.Object, _    ByVal RowID As System.Integer, _    ByVal Text As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwCalloutHandler Dim pManipulator As System.Object Dim RowID As System.Integer Dim Text As System.String Dim value As System.Boolean   value = instance.OnStringValueChanged(pManipulator, RowID, Text) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool OnStringValueChanged(     System.object pManipulator,    System.int RowID,    System.string Text ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool OnStringValueChanged(  &   System.Object^ pManipulator, &   System.int RowID, &   System.String^ Text ) ``` | |

#### Parameters

*pManipulator*
:   ICallout object whose text was edited

*RowID*
:   Row in which the text was edi

*Text*
:   New text of RowID

#### Return Value

True to use updated text in RowID, false to use original text in RowID

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwCalloutHandler::OnStringValueChanged.

# ![](dotnetimages/collapse.gif)Example

[Create Multi-row Callouts (VBA)](Create_Multi-row_Callouts_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISwCalloutHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwCalloutHandler.html)

[ISwCalloutHandler Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwCalloutHandler_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0