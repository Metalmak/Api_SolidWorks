<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7~OnPopupMenuItemUpdate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnPopupMenuItemUpdate Method (IPropertyManagerPage2Handler7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler7 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7.html) : OnPopupMenuItemUpdate Method (IPropertyManagerPage2Handler7) |

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

*retval*
:   State of the specified unique user-defined pop-up menu item:

    * 0 - Not selected (i.e., not checked) and disabled (i.e., grayed out)* 1 - Not selected and enabled

        * 2 - Selected (i.e., checked) and disabled

          * 3 - Selected and enabled

Obsoleted. Superseded by [IPropertyManagerPage2Handler8::OnPopupMenuItemUpdate.](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler8~OnPopupMenuItemUpdate.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnPopupMenuItemUpdate( _    ByVal Id As System.Integer, _    ByRef retval As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler7 Dim Id As System.Integer Dim retval As System.Integer   instance.OnPopupMenuItemUpdate(Id, retval) ``` | |

| C# |  |
| --- | --- |
| ``` void OnPopupMenuItemUpdate(     System.int Id,    ref System.int retval ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnPopupMenuItemUpdate(  &   System.int Id, &   System.int% retval ) ``` | |

#### Parameters

*Id*
:   Unique user-defined ID for a pop-up menu item (see IPropertyManagerPage2::AddMenuPopupItem)

*retval*
:   State of the specified unique user-defined pop-up menu item:

    * 0 - Not selected (i.e., not checked) and disabled (i.e., grayed out)* 1 - Not selected and enabled

        * 2 - Selected (i.e., checked) and disabled

          * 3 - Selected and enabled

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler7::OnPopupMenuItemUpdate.

# ![](dotnetimages/collapse.gif)Remarks

Thus, this method:

* processes a request for the state of the specified pop-up menu item associated with the PropertyManager page.* passes the state back to SOLIDWORKS.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler7 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7.html)

[IPropertyManagerPage2Handler7 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7_members.html)

[IPropertyManagerPage2Handler7::OnPopupMenuItem Method](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7~OnPopupMenuItem.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0