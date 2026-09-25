<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8~OnLostFocus.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnLostFocus Method (IPropertyManagerPage2Handler8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler8 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8.html) : OnLostFocus Method (IPropertyManagerPage2Handler8) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Id*
:   ID of the control that lost focus

Obsolete. Superseded by [IPropertyManagerPage2Handler9::OnLostFocus](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler9~OnLostFocus.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnLostFocus( _    ByVal Id As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler8 Dim Id As System.Integer   instance.OnLostFocus(Id) ``` | |

| C# |  |
| --- | --- |
| ``` void OnLostFocus(     System.int Id ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnLostFocus(  &   System.int Id ) ``` | |

#### Parameters

*Id*
:   ID of the control that lost focus

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler8::OnLostFocus.

# ![](dotnetimages/collapse.gif)Remarks

To handle selection box focus, use [IPropertyManagerPage2Handler8::OnSelectionboxFocusChanged](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler8~OnSelectionboxFocusChanged.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler8 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8.html)

[IPropertyManagerPage2Handler8 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0