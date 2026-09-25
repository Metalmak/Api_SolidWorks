<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveItemFromThirdPartyPopupMenu.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RemoveItemFromThirdPartyPopupMenu Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : RemoveItemFromThirdPartyPopupMenu Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RegisterId*
:   :   ID of the shortcut menu from [ISldWorks::RegisterThirdPartyPopupMenu](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RegisterThirdPartyPopupMenu.html)

*DocType*
:   :   Document type where to display the shortcut menu, as defined in swDocumentTypes\_e

*Item*
:   Name of the shortcut menu item

*IconIndex*
:   1-based index of the icon (see **Remarks**)

Removes a menu item and icon from a third-party pop-up (shortcut) menu.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RemoveItemFromThirdPartyPopupMenu( _    ByVal RegisterId As System.Integer, _    ByVal DocType As System.Integer, _    ByVal Item As System.String, _    ByVal IconIndex As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim RegisterId As System.Integer Dim DocType As System.Integer Dim Item As System.String Dim IconIndex As System.Integer Dim value As System.Boolean   value = instance.RemoveItemFromThirdPartyPopupMenu(RegisterId, DocType, Item, IconIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool RemoveItemFromThirdPartyPopupMenu(     System.int RegisterId,    System.int DocType,    System.string Item,    System.int IconIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool RemoveItemFromThirdPartyPopupMenu(  &   System.int RegisterId, &   System.int DocType, &   System.String^ Item, &   System.int IconIndex ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RegisterId*
:   :   ID of the shortcut menu from [ISldWorks::RegisterThirdPartyPopupMenu](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RegisterThirdPartyPopupMenu.html)

*DocType*
:   :   Document type where to display the shortcut menu, as defined in swDocumentTypes\_e

*Item*
:   Name of the shortcut menu item

*IconIndex*
:   1-based index of the icon (see **Remarks**)

#### Return Value

True if the shortcut menu item or icon is removed, false if not

# ![](dotnetimages/collapse.gif)Example

[Add Shortcut Menus to Add-ins (VB.NET)](Add_Shortcut_Menus_to_Add-ins_VBNET.htm)

[Add Shortcut Menus to Add-ins (C#)](Add_Shortcut_Menus_to_Add-ins_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To remove:

* a menu item, specify a valid name for Item only. If you specify both Item and IconIndex, only Item is evaluated; IconIndex is ignored.* a menu bar icon, specify an empty string for Item and pass the 1-based index value of the icon for IconIndex.

Read about Add-in Shortcut Menus.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::AddItemToThirdPartyPopupMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddItemToThirdPartyPopupMenu.html)

[ISldWorks::SetThirdPartyPopupMenuState Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetThirdPartyPopupMenuState.html)

[ISldWorks::ShowThirdPartyPopupMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ShowThirdPartyPopupMenu.html)

[ISldWorks::AddItemToThirdPartyPopupMenu2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddItemToThirdPartyPopupMenu2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0