<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7~OnLostFocus.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnLostFocus Method (IPropertyManagerPage2Handler7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler7 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7.html) : OnLostFocus Method (IPropertyManagerPage2Handler7) |

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

Obsoleted. Superseded by [IPropertyManagerPage2Handler8::OnLostFocus](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler8~OnLostFocus.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnLostFocus( _    ByVal Id As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler7 Dim Id As System.Integer   instance.OnLostFocus(Id) ``` | |

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

See PropertyManagerPage2Handler7::OnLostFocus.

# ![](dotnetimages/collapse.gif)Remarks

To handle selection box focus, use [IPropertyManagerPage2Handler7::OnSelectionboxFocusChanged](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler7~OnSelectionboxFocusChanged.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler7 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7.html)

[IPropertyManagerPage2Handler7 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7_members.html)

[IPropertyManagerPage2Handler7::OnGainedFocus Method](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7~OnGainedFocus.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0