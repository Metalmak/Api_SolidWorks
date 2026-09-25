<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9~OnPopupMenuItemUpdate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnPopupMenuItemUpdate Method (IPropertyManagerPage2Handler9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler9 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html) : OnPopupMenuItemUpdate Method (IPropertyManagerPage2Handler9) |

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

    * 0 - Not selected (i.e., not checked) and disabled (i.e., grayed out)* 1 - Not selected and enabled* 2 - Selected (i.e., checked) and disabled

          * 3 - Selected and enabled

When Windows attempts to select or deselect and enable or disable the pop-up menu item, SOLIDWORKS calls this method to get the state of the menu item from the add-in.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnPopupMenuItemUpdate( _    ByVal Id As System.Integer, _    ByRef retval As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler9 Dim Id As System.Integer Dim retval As System.Integer   instance.OnPopupMenuItemUpdate(Id, retval) ``` | |

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

    * 0 - Not selected (i.e., not checked) and disabled (i.e., grayed out)* 1 - Not selected and enabled* 2 - Selected (i.e., checked) and disabled

          * 3 - Selected and enabled

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler9::OnPopupMenuItemUpdate.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPage2Handler9](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method:

* processes a request for the state of the specified pop-up menu item associated with the PropertyManager page.* passes the state back to SOLIDWORKS.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler9 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html)

[IPropertyManagerPage2Handler9 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9_members.html)

[IPropertyManagerPage2Handler9::OnPopupMenuItem Method](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9~OnPopupMenuItem.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0