<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8~OnSelectionboxFocusChanged.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnSelectionboxFocusChanged Method (IPropertyManagerPage2Handler8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler8 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8.html) : OnSelectionboxFocusChanged Method (IPropertyManagerPage2Handler8) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Id*
:   ID of this selection box with focus

Obsolete. Superseded by [IPropertyManagerPage2Handler9::OnSelectionboxFocusChanged](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler9~OnSelectionboxFocusChanged.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnSelectionboxFocusChanged( _    ByVal Id As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler8 Dim Id As System.Integer   instance.OnSelectionboxFocusChanged(Id) ``` | |

| C# |  |
| --- | --- |
| ``` void OnSelectionboxFocusChanged(     System.int Id ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnSelectionboxFocusChanged(  &   System.int Id ) ``` | |

#### Parameters

*Id*
:   ID of this selection box with focus

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler8::OnSelectionboxFocusChanged.

# ![](dotnetimages/collapse.gif)Remarks

A PropertyManager page often has more than one selection list. The focus is always on the active selection list. When the focus changes to another selection list, this subroutine is called. If there is only one selection list on the page, then the focus never leaves it, and this subroutine is never called.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler8 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8.html)

[IPropertyManagerPage2Handler8 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0