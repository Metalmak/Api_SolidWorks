<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddItemToThirdPartyPopupMenu2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddItemToThirdPartyPopupMenu2 Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : AddItemToThirdPartyPopupMenu2 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RegisterId*
:   ID of shortcut menu from [ISldWorks::RegisterThirdPartyPopupMenu](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RegisterThirdPartyPopupMenu.html)

*DocType*
:   Document type where to display shortcut menu, as defined in swDocumentTypes\_e

*Item*
:   Unique display name of shortcut menu item (see **Remarks**); specify an empty string if adding an icon to the menu bar

*Identifier*
:   ID of the add-in; value of the Cookie argument passed by ISwAddin::ConnectToSW

*CallbackFunction*
:   Function called when user clicks the shortcut menu item; specify an empty string if MenuItemTypeOption is:

    * swMenuItemType\_e.swMenuItemType\_Break* swMenuItemType\_e.swMenuItemType\_Separator

    (see **Remarks**)

*EnableFunction*
:   Optional function that controls the state of the shortcut menu item

    If specified, SOLIDWORKS:

    1. calls this function before displaying the menu

       - displays the menu item according to the return value of this function

    | If EnableFunction returns... | **Then SOLIDWORKS...** |
    | --- | --- |
    | 0 | Deselects and disables the menu item |
    | 1 | Deselects and enables the menu item; this is the default menu state if EnableFunction is not specified |
    | 2 | Selects and disables the menu item |
    | 3 | Selects and enables the menu item |

    Specify an empty string if MenuItemTypeOption is:

    * swMenuItemType\_e.swMenuItemType\_Break* swMenuItemType\_e.swMenuItemType\_Separator

    (see **Remarks**)

*CustomName*
:   Empty string

*HintString*
:   Text to display in the SOLIDWORKS status bar when users move the mouse over this shortcut menu item

*BitmapFileName*
:   Path and filename of bitmap for icons (menu bar or menu item)

    Specify an empty string if MenuItemTypeOption is:

    * swMenuItemType\_e.swMenuItemType\_Break* swMenuItemType\_e.swMenuItemType\_Separator

*MenuItemTypeOption*
:   Type of menu item as defined in swMenuItemType\_e

Adds menu items to a pop-up (shortcut) menu in a SOLIDWORKS add-in.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddItemToThirdPartyPopupMenu2( _    ByVal RegisterId As System.Integer, _    ByVal DocType As System.Integer, _    ByVal Item As System.String, _    ByVal Identifier As System.Integer, _    ByVal CallbackFunction As System.String, _    ByVal EnableFunction As System.String, _    ByVal CustomName As System.String, _    ByVal HintString As System.String, _    ByVal BitmapFileName As System.String, _    ByVal MenuItemTypeOption As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim RegisterId As System.Integer Dim DocType As System.Integer Dim Item As System.String Dim Identifier As System.Integer Dim CallbackFunction As System.String Dim EnableFunction As System.String Dim CustomName As System.String Dim HintString As System.String Dim BitmapFileName As System.String Dim MenuItemTypeOption As System.Integer Dim value As System.Boolean   value = instance.AddItemToThirdPartyPopupMenu2(RegisterId, DocType, Item, Identifier, CallbackFunction, EnableFunction, CustomName, HintString, BitmapFileName, MenuItemTypeOption) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddItemToThirdPartyPopupMenu2(     System.int RegisterId,    System.int DocType,    System.string Item,    System.int Identifier,    System.string CallbackFunction,    System.string EnableFunction,    System.string CustomName,    System.string HintString,    System.string BitmapFileName,    System.int MenuItemTypeOption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddItemToThirdPartyPopupMenu2(  &   System.int RegisterId, &   System.int DocType, &   System.String^ Item, &   System.int Identifier, &   System.String^ CallbackFunction, &   System.String^ EnableFunction, &   System.String^ CustomName, &   System.String^ HintString, &   System.String^ BitmapFileName, &   System.int MenuItemTypeOption ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RegisterId*
:   ID of shortcut menu from [ISldWorks::RegisterThirdPartyPopupMenu](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RegisterThirdPartyPopupMenu.html)

*DocType*
:   Document type where to display shortcut menu, as defined in swDocumentTypes\_e

*Item*
:   Unique display name of shortcut menu item (see **Remarks**); specify an empty string if adding an icon to the menu bar

*Identifier*
:   ID of the add-in; value of the Cookie argument passed by ISwAddin::ConnectToSW

*CallbackFunction*
:   Function called when user clicks the shortcut menu item; specify an empty string if MenuItemTypeOption is:

    * swMenuItemType\_e.swMenuItemType\_Break* swMenuItemType\_e.swMenuItemType\_Separator

    (see **Remarks**)

*EnableFunction*
:   Optional function that controls the state of the shortcut menu item

    If specified, SOLIDWORKS:

    1. calls this function before displaying the menu

       - displays the menu item according to the return value of this function

    | If EnableFunction returns... | **Then SOLIDWORKS...** |
    | --- | --- |
    | 0 | Deselects and disables the menu item |
    | 1 | Deselects and enables the menu item; this is the default menu state if EnableFunction is not specified |
    | 2 | Selects and disables the menu item |
    | 3 | Selects and enables the menu item |

    Specify an empty string if MenuItemTypeOption is:

    * swMenuItemType\_e.swMenuItemType\_Break* swMenuItemType\_e.swMenuItemType\_Separator

    (see **Remarks**)

*CustomName*
:   Empty string

*HintString*
:   Text to display in the SOLIDWORKS status bar when users move the mouse over this shortcut menu item

*BitmapFileName*
:   Path and filename of bitmap for icons (menu bar or menu item)

    Specify an empty string if MenuItemTypeOption is:

    * swMenuItemType\_e.swMenuItemType\_Break* swMenuItemType\_e.swMenuItemType\_Separator

*MenuItemTypeOption*
:   Type of menu item as defined in swMenuItemType\_e

#### Return Value

True if the shortcut menu item is added, false if not

# ![](dotnetimages/collapse.gif)Example

| VB.NET | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` 'To create and register a shortcut menu:    registerID = SwApp.RegisterThirdPartyPopupMenu()     'To add an actionable menu item to a shortcut menu:    resultCode = SwApp.AddItemToThirdPartyPopupMenu2(    registerID,     CInt(swDocumentTypes_e.swDocPART),     "Test1",     addinID,     "TestCallback",     "EnableTest",     "",     "Test1",     cmdGroup.SmallMainIcon,     CInt(swMenuItemType_e.swMenuItemType_Default))     'To add a separator bar to a shortcut menu     resultCode = SwApp.AddItemToThirdPartyPopupMenu2(    registerID,     CInt(swDocumentTypes_e.swDocPART),     "Separator1",    addinID     "",     "",     "",     "",     "",    CInt(swMenuItemType_e.swMenuItemType_Separator))     'To add a section title or break to a shortcut menu:    resultCode = SwApp.AddItemToThirdPartyPopupMenu2(    registerID,     CInt(swDocumentTypes_e.swDocPART),     "Menu Break",     addinID,     "",     "",     "",     "",     "",     CInt(swMenuItemType_e.swMenuItemType_Break))  'To add an icon to the menu bar above a shortcut menu:    resultCode = SwApp.AddItemToThirdPartyPopupMenu2(    registerID,     CInt(swDocumentTypes_e.swDocPART),     "",     addinID,     "TestCallback",     "EnableTest",     "",     "NoOp",     cmdGroup.SmallMainIcon,     CInt(swMenuItemType_e.swMenuItemType_Default)) ``` | |

# ![](dotnetimages/collapse.gif)Example

[Add Shortcut Menus to Add-ins (VB.NET)](Add_Shortcut_Menus_to_Add-ins_VBNET.htm)

[Add Shortcut Menus to Add-ins (C#)](Add_Shortcut_Menus_to_Add-ins_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

See Add-in Callback and Enable Methods to learn how to specify CallbackFunction and EnableFunction.

Read about Add-in Shortcut Menus.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::AddItemToThirdPartyPopupMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddItemToThirdPartyPopupMenu.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0