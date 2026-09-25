<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddItemToThirdPartyPopupMenu.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddItemToThirdPartyPopupMenu Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : AddItemToThirdPartyPopupMenu Method (ISldWorks) |

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
:   Name of shortcut menu item (see **Remarks**)

*CallbackFcnAndModule*
:   Function called when user clicks the shortcut menu item (see **Remarks**)

*CustomName*
:   Empty string

*HintString*
:   Text to display in the SOLIDWORKS status bar when users move the mouse over this shortcut menu item

*BitmapFileName*
:   Path and filename of the bitmap

*MenuItemTypeOption*
:   Menu item as defined in swMenuItemType\_e

Adds menu items to a pop-up (shortcut) menu in a C++ SOLIDWORKS add-in.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddItemToThirdPartyPopupMenu( _    ByVal RegisterId As System.Integer, _    ByVal DocType As System.Integer, _    ByVal Item As System.String, _    ByVal CallbackFcnAndModule As System.String, _    ByVal CustomName As System.String, _    ByVal HintString As System.String, _    ByVal BitmapFileName As System.String, _    ByVal MenuItemTypeOption As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim RegisterId As System.Integer Dim DocType As System.Integer Dim Item As System.String Dim CallbackFcnAndModule As System.String Dim CustomName As System.String Dim HintString As System.String Dim BitmapFileName As System.String Dim MenuItemTypeOption As System.Integer Dim value As System.Boolean   value = instance.AddItemToThirdPartyPopupMenu(RegisterId, DocType, Item, CallbackFcnAndModule, CustomName, HintString, BitmapFileName, MenuItemTypeOption) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddItemToThirdPartyPopupMenu(     System.int RegisterId,    System.int DocType,    System.string Item,    System.string CallbackFcnAndModule,    System.string CustomName,    System.string HintString,    System.string BitmapFileName,    System.int MenuItemTypeOption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddItemToThirdPartyPopupMenu(  &   System.int RegisterId, &   System.int DocType, &   System.String^ Item, &   System.String^ CallbackFcnAndModule, &   System.String^ CustomName, &   System.String^ HintString, &   System.String^ BitmapFileName, &   System.int MenuItemTypeOption ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RegisterId*
:   ID of shortcut menu from [ISldWorks::RegisterThirdPartyPopupMenu](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RegisterThirdPartyPopupMenu.html)

*DocType*
:   Document type where to display shortcut menu, as defined in swDocumentTypes\_e

*Item*
:   Name of shortcut menu item (see **Remarks**)

*CallbackFcnAndModule*
:   Function called when user clicks the shortcut menu item (see **Remarks**)

*CustomName*
:   Empty string

*HintString*
:   Text to display in the SOLIDWORKS status bar when users move the mouse over this shortcut menu item

*BitmapFileName*
:   Path and filename of the bitmap

*MenuItemTypeOption*
:   Menu item as defined in swMenuItemType\_e

#### Return Value

True if the shortcut menu item is added, false if not

# ![](dotnetimages/collapse.gif)Example

| C++ | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` To add a section title or break to the shortcut menu:  iSwApp->AddItemToThirdPartyPopupMenu ( registerIdPMenu1, swDocPART, CComBSTR(_T("Menu Break")), CComBSTR(_T("")), CComBSTR(_T("")), CComBSTR(_T("")), CComBSTR(_T("")), swMenuItemType_Break, &itemAdded );  To add an icon to a menu bar above the shortcut menu:  iSwApp->AddItemToThirdPartyPopupMenu ( registerIdPMenu1, swDocPART, CComBSTR(_T("")), CComBSTR(_T("UserPopupMenus.dll@UserItem1_Menu1_Callback")), CComBSTR(_T("")), CComBSTR(_T("UserItem1_Menu1_Callback_hint")), UserItem1_Menu1_bitmapFile, swMenuItemType_Default, &itemAdded );  To add an actionable item to the shortcut menu:  iSwApp->AddItemToThirdPartyPopupMenu ( registerIdPMenu1, swDocPART, CComBSTR(_T("UserItem1_Menu1_Callback")), CComBSTR(_T("UserPopupMenus.dll@UserItem1_Menu1_Callback")), CComBSTR(_T("")), CComBSTR(_T("UserItem1_Menu1_Callback_hint")), UserItem1_Menu1_bitmapFile, swMenuItemType_Default, &itemAdded );  To add a separator bar to the shortcut menu:  iSwApp->AddItemToThirdPartyPopupMenu ( registerIdPMenu1, swDocPART, CComBSTR(_T("")), CComBSTR(_T("")), CComBSTR(_T("")), CComBSTR(_T("")), CComBSTR(_T("")), swMenuItemType_Separator, &itemAdded ); ``` | |

# ![](dotnetimages/collapse.gif)Remarks

This method is supported in C++ applications only, and it only works in C++ applications implemented as DLLs, not as EXEs.

Read about Add-in Shortcut Menus.

The CallbackFcnAndModule argument specifies which function to call when this shortcut menu item is selected by the user. The syntax is as follows:

"dllname@function@updatefunction"

where:

|  |  |
| --- | --- |
| dllname | Name of your library as specified in the project .def file. The actual DLL filename and the definition in the .def file must be the same. |
| function | Name of the function that gets called when the user clicks the shortcut menu item. This function must also be declared as an EXPORT in your .def file.  See Add-in Callback and Enable Methods to learn how to implement your function. |
| updatefunction | Optional argument that controls the state of the shortcut menu item. If specified, then SOLIDWORKS calls this function before the shortcut menu item is displayed. Define your updatefunction to return an integer and declare it as an EXPORT or included in your .def file.  The display of the third-party shortcut menu item is controlled by the return value of the function as follows:   * return 0 - Unchecked and disabled. * return 1 - Unchecked and enabled. This is the default menu state if no updatefunction is specified. * return 2 - Checked and disabled. * return 3 - Checked and enabled.   See Add-in Callback and Enable Methods to learn how to implement your updatefunction. |

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::AddItemToThirdPartyPopupMenu2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddItemToThirdPartyPopupMenu2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0