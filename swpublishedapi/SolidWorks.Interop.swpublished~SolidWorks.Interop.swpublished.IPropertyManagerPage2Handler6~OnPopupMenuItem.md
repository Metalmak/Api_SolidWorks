<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6~OnPopupMenuItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnPopupMenuItem Method (IPropertyManagerPage2Handler6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler6 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6.html) : OnPopupMenuItem Method (IPropertyManagerPage2Handler6) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Id*
:   Unique user-defined ID for a pop-up menu item (see IPropertyManagerPage2::AddMenuPopupItem)

Obsoleted. Superseded by [IPropertyManagerPage2Handler7::OnPopupMenuItem](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler7~OnPopupMenuItem.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnPopupMenuItem( _    ByVal Id As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler6 Dim Id As System.Integer   instance.OnPopupMenuItem(Id) ``` | |

| C# |  |
| --- | --- |
| ``` void OnPopupMenuItem(     System.int Id ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnPopupMenuItem(  &   System.int Id ) ``` | |

#### Parameters

*Id*
:   Unique user-defined ID for a pop-up menu item (see IPropertyManagerPage2::AddMenuPopupItem)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler6::OnPopupMenuItem.

# ![](dotnetimages/collapse.gif)Remarks

The add-in should then perform the appropriate action.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler6 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6.html)

[IPropertyManagerPage2Handler6 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6_members.html)

[IPropertyManagerPage2Handler6::OnPopupMenuItemUpdate Method](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6~OnPopupMenuItemUpdate.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0