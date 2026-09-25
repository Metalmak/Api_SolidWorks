<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenu.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddMenu Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : AddMenu Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DocType*
:   Document type to add the menu item as defined by swDocumentTypes\_e

*Menu*
:   Name of menu item to add, including any parent menu names, e.g., subMenuString@menuString

*Position*
:   Specifies the position where to add the new menu item; 0 = first position and 1 = end of the parent menu (see **Remarks**)

Adds a menu item to a SOLIDWORKS menu for DLL applications.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddMenu( _    ByVal DocType As System.Integer, _    ByVal Menu As System.String, _    ByVal Position As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim DocType As System.Integer Dim Menu As System.String Dim Position As System.Integer Dim value As System.Integer   value = instance.AddMenu(DocType, Menu, Position) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddMenu(     System.int DocType,    System.string Menu,    System.int Position ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddMenu(  &   System.int DocType, &   System.String^ Menu, &   System.int Position ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DocType*
:   Document type to add the menu item as defined by swDocumentTypes\_e

*Menu*
:   Name of menu item to add, including any parent menu names, e.g., subMenuString@menuString

*Position*
:   Specifies the position where to add the new menu item; 0 = first position and 1 = end of the parent menu (see **Remarks**)

#### Return Value

1 if menu item is added successfully added or 0 if adding the menu item failed

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::AddMenu.

# ![](dotnetimages/collapse.gif)Example

[Add Menu and Menu Item (C#)](Add_Menu_and_Menu_Item_Example_CSharp.htm)

[Add Menu and Menu Item (VB.NET)](Add_Menu_and_Menu_Item_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

If the name of a parent menu is not specified in Menu, then:

* the menu item appears on the **Tools** menu below the **XPress products** menu item.* Position is ignored.

Menus items are automatically created at the end of the parent menu when using [ISldWorks::AddMenuItem5](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenuItem5.html). Therefore, if your menu structure is created using sequential calls to SldWorks::AddMenuItem5, then all the menu items are positioned based on their order of creation.

This method is only required when a menu needs to be placed into an existing menu at a specific position.

Read about Add-in Shortcut Menus.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::AddMenuPopupItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenuPopupItem2.html)

[ISldWorks::AddToolbar4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddToolbar4.html)

[ISldWorks::AddToolbarCommand2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddToolbarCommand2.html)

[ISldWorks::RemoveFromMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveFromMenu.html)

[ISldWorks::RemoveFromPopupMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveFromPopupMenu.html)

[ISldWorks::RemoveMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveMenu.html)

[ISldWorks::RemoveMenuPopupItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveMenuPopupItem2.html)

[ISldWorks::RemoveToolbar2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveToolbar2.html)

[ISldWorks::GetLocalizedMenuName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetLocalizedMenuName.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207