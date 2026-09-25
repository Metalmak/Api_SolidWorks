<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSelectionbox~AddMenuPopupItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddMenuPopupItem Method (IPropertyManagerPageSelectionbox) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageSelectionbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSelectionbox.html) : AddMenuPopupItem Method (IPropertyManagerPageSelectionbox) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ID*
:   Unique user-defined value for this pop-up menu item

*ItemText*
:   Text for pop-up menu item

*DocumentType*
:   Document types for which this pop-up menu item is displayed as defined in swDocumentTypes\_e

*HintText*
:   Text displayed in the SOLIDWORKS status bar when the user moves the cursor over this pop-up menu item

Adds a menu item to the pop-up menu for this selection box of the PropertyManager page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddMenuPopupItem( _    ByVal ID As System.Integer, _    ByVal ItemText As System.String, _    ByVal DocumentType As System.Integer, _    ByVal HintText As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageSelectionbox Dim ID As System.Integer Dim ItemText As System.String Dim DocumentType As System.Integer Dim HintText As System.String Dim value As System.Boolean   value = instance.AddMenuPopupItem(ID, ItemText, DocumentType, HintText) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddMenuPopupItem(     System.int ID,    System.string ItemText,    System.int DocumentType,    System.string HintText ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddMenuPopupItem(  &   System.int ID, &   System.String^ ItemText, &   System.int DocumentType, &   System.String^ HintText ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ID*
:   Unique user-defined value for this pop-up menu item

*ItemText*
:   Text for pop-up menu item

*DocumentType*
:   Document types for which this pop-up menu item is displayed as defined in swDocumentTypes\_e

*HintText*
:   Text displayed in the SOLIDWORKS status bar when the user moves the cursor over this pop-up menu item

#### Return Value

True if the pop-up menu item is added, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageSelectionbox::AddMenuPopupItem.

# ![](dotnetimages/collapse.gif)Remarks

This method requires that you implement these IPropertyManagerPage2Handler5 methods:

* IPropertyManagerPage2Handler5::OnPopupMenuItem. When the user selects a pop-up menu item, this method determines which item was selected. The add-in should then perform the appropriate action.

* IPropertyManagerPage2Handler5::OnPopupMenuItemUpdate. When Windows attempts to select or deselect and enable or disable the pop-up menu item, SOLIDWORKS calls IPropertyManagerPage2Handler5::OnPopupMenuItemUpdate to get the state of the pop-up menu item from the add-in. Thus, IPropertyManagerPage2Handler5::OnPopupMenuItemUpdate:

  + Processes a request for the state of the specified pop-up menu item associated with the PropertyManager page.

    + Passes the state back to SOLIDWORKS.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageSelectionbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSelectionbox.html)

[IPropertyManagerPageSelectionbox Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSelectionbox_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0