<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenuItem4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddMenuItem4 Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : AddMenuItem4 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DocumentType*
:   Document type to add the menu item as defined by swDocumentTypes\_e

*Cookie*
:   Cookie as defined in ISwAddin::ConnectToSW

*MenuItem*
:   Menu string ("menuItem@menuString"); SOLIDWORKS creates menu items only if they do not already exist

    NOTES:

    * If you do not specify menuString, then the menu item appears on the Tools menu below the **Xpress Products** menu item.* Use the & symbol to include an accelerator key, e.g., "MyItem@&File" adds MyItem to the File menu with an accelerator key. To display the accelerator key, press the Alt key. The accelerator key is underlined.

*Position*
:   Position where to add the new menu item; the first item is at position 0; if -1 is specified for Position, then the new menu item is added to the bottom of the list; this argument specifies the position of the menu item in relation to its immediate parent menu.

*MenuCallback*
:   Function to call when this menu item is selected (see **Remarks**)

*MenuEnableMethod*
:   Optional function that controls the state of the menu item (See **Remarks**)

    If specified:

    * SOLIDWORKS calls this function before displaying the menu.

      * Display of the menu item is controlled by the return value of MenuEnableMethod.

    | If MenuEnableMethod returns... | **Then SOLIDWORKS...** |
    | --- | --- |
    | 0 | Deselects and disables the menu item |
    | 1 | Deselects and enables the menu item; this is the default menu state if no update function is specified |
    | 2 | Selects and disables the menu item |
    | 3 | Selects and enables the menu item |

*HintString*
:   Text to show in the SOLIDWORKS status bar when the user moves the pointer over this menu item; if you specify HintString, then it must be preceded by a comma

*BitmapFilePath*
:   Path and filename of bitmap

Obsolete. Superseded by [ISldWorks::AddMenuItem5](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenuItem5.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddMenuItem4( _    ByVal DocumentType As System.Integer, _    ByVal Cookie As System.Integer, _    ByVal MenuItem As System.String, _    ByVal Position As System.Integer, _    ByVal MenuCallback As System.String, _    ByVal MenuEnableMethod As System.String, _    ByVal HintString As System.String, _    ByVal BitmapFilePath As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim DocumentType As System.Integer Dim Cookie As System.Integer Dim MenuItem As System.String Dim Position As System.Integer Dim MenuCallback As System.String Dim MenuEnableMethod As System.String Dim HintString As System.String Dim BitmapFilePath As System.String Dim value As System.Integer   value = instance.AddMenuItem4(DocumentType, Cookie, MenuItem, Position, MenuCallback, MenuEnableMethod, HintString, BitmapFilePath) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddMenuItem4(     System.int DocumentType,    System.int Cookie,    System.string MenuItem,    System.int Position,    System.string MenuCallback,    System.string MenuEnableMethod,    System.string HintString,    System.string BitmapFilePath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddMenuItem4(  &   System.int DocumentType, &   System.int Cookie, &   System.String^ MenuItem, &   System.int Position, &   System.String^ MenuCallback, &   System.String^ MenuEnableMethod, &   System.String^ HintString, &   System.String^ BitmapFilePath ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DocumentType*
:   Document type to add the menu item as defined by swDocumentTypes\_e

*Cookie*
:   Cookie as defined in ISwAddin::ConnectToSW

*MenuItem*
:   Menu string ("menuItem@menuString"); SOLIDWORKS creates menu items only if they do not already exist

    NOTES:

    * If you do not specify menuString, then the menu item appears on the Tools menu below the **Xpress Products** menu item.* Use the & symbol to include an accelerator key, e.g., "MyItem@&File" adds MyItem to the File menu with an accelerator key. To display the accelerator key, press the Alt key. The accelerator key is underlined.

*Position*
:   Position where to add the new menu item; the first item is at position 0; if -1 is specified for Position, then the new menu item is added to the bottom of the list; this argument specifies the position of the menu item in relation to its immediate parent menu.

*MenuCallback*
:   Function to call when this menu item is selected (see **Remarks**)

*MenuEnableMethod*
:   Optional function that controls the state of the menu item (See **Remarks**)

    If specified:

    * SOLIDWORKS calls this function before displaying the menu.

      * Display of the menu item is controlled by the return value of MenuEnableMethod.

    | If MenuEnableMethod returns... | **Then SOLIDWORKS...** |
    | --- | --- |
    | 0 | Deselects and disables the menu item |
    | 1 | Deselects and enables the menu item; this is the default menu state if no update function is specified |
    | 2 | Selects and disables the menu item |
    | 3 | Selects and enables the menu item |

*HintString*
:   Text to show in the SOLIDWORKS status bar when the user moves the pointer over this menu item; if you specify HintString, then it must be preceded by a comma

*BitmapFilePath*
:   Path and filename of bitmap

#### Return Value

SOLIDWORKS runtime command ID if successful, -1 if unsuccessful

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::AddMenuItem4.

# ![](dotnetimages/collapse.gif)Remarks

See Add-in Callback and Enable Methods to learn how to specify MenuCallback and MenuEnableMethod.

For information about using this method with the ISwAddin object, see Using ISwAddin to Create a SOLIDWORKS Add-in.

The bitmap must be 16w x 16h x 256 colors.

You can add a new menu item to any one of the four SOLIDWORKS frames (main, part, assembly, or drawing). To do this, call this method with the appropriate argument in the DocumentType parameter. For example, if you want your menu item to be available when a part document is active, then call this method and pass swDocPART as the first argument. After you have added your menu item to the part frame, you do not need to do it again during the current SOLIDWORKS session. Once a part document is activated by the user, SOLIDWORKS automatically displays your menu item.

To add a menu separator:

* leave the text for the menu item blank, so that the menu string for the MenuItem argument starts with the at-sign symbol ( @):

  "@subMenuString@menuString"

  * specify an existing method for the MenuCallback argument. This method is never called, so its implementation can be empty.

    * specify empty strings for the MenuEnableMethod, HintString, and bitmapFilePath arguments.

Read about Add-in Shortcut Menus.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::AddMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenu.html)

[ISldWorks::AddMenuPopupItem3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenuPopupItem3.html)

[ISldWorks::AddToolbar4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddToolbar4.html)

[ISldWorks::RemoveMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveMenu.html)

[ISldWorks::RemoveFromMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveFromMenu.html)

[ISldWorks::RemoveMenuPopupItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveMenuPopupItem2.html)

[ISldWorks::RemoveToolbar2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveToolbar2.html)

[ISldWorks::GetLocalizedMenuName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetLocalizedMenuName.html)

[ISldWorks::RemoveFromPopupMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveFromPopupMenu.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0