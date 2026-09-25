<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuPopupIcon2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddMenuPopupIcon2 Method (IFrame) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFrame Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame.html) : AddMenuPopupIcon2 Method (IFrame) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DocType*
:   Document type whose context-sensitive menus display the icon

*SelectType*
:   Selection type whose context-sensitive menus display the icon

*HintString*
:   Text displayed in the SOLIDWORKS status bar when the user moves the pointer over the icon

*Identifier*
:   ID of the add-in; value of the Cookie argument passed by ISwAddin::ConnectToSW

*CallbackFunction*
:   Function called when user clicks the context-sensitive menu icon (**see Remarks**)

*CallbackUpdateFunction*
:   Optional function that controls the state of the icon; if specified, then SOLIDWORKS calls this function before displaying the icon

    | If CallbackUpdateFunction returns... | Then SOLIDWORKS... |
    | --- | --- |
    | 0 | Deselects and disables the item |
    | 1 | Deselects and enables the item; this is the default state if no update function is specified |
    | 4 | Hides the item |

    (see **Remarks**)

*CustomNames*
:   Names of custom feature types (see **Remarks**)

*BitmapFilePath*
:   Path and file name of the bitmap for the context-sensitive menu icon

Obsolete. Superseded by [IFrame::AddMenuPopupIcon3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuPopupIcon3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddMenuPopupIcon2( _    ByVal DocType As System.Integer, _    ByVal SelectType As System.Integer, _    ByVal HintString As System.String, _    ByVal Identifier As System.Integer, _    ByVal CallbackFunction As System.String, _    ByVal CallbackUpdateFunction As System.String, _    ByVal CustomNames As System.String, _    ByVal BitmapFilePath As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFrame Dim DocType As System.Integer Dim SelectType As System.Integer Dim HintString As System.String Dim Identifier As System.Integer Dim CallbackFunction As System.String Dim CallbackUpdateFunction As System.String Dim CustomNames As System.String Dim BitmapFilePath As System.String Dim value As System.Boolean   value = instance.AddMenuPopupIcon2(DocType, SelectType, HintString, Identifier, CallbackFunction, CallbackUpdateFunction, CustomNames, BitmapFilePath) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddMenuPopupIcon2(     System.int DocType,    System.int SelectType,    System.string HintString,    System.int Identifier,    System.string CallbackFunction,    System.string CallbackUpdateFunction,    System.string CustomNames,    System.string BitmapFilePath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddMenuPopupIcon2(  &   System.int DocType, &   System.int SelectType, &   System.String^ HintString, &   System.int Identifier, &   System.String^ CallbackFunction, &   System.String^ CallbackUpdateFunction, &   System.String^ CustomNames, &   System.String^ BitmapFilePath ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DocType*
:   Document type whose context-sensitive menus display the icon

*SelectType*
:   Selection type whose context-sensitive menus display the icon

*HintString*
:   Text displayed in the SOLIDWORKS status bar when the user moves the pointer over the icon

*Identifier*
:   ID of the add-in; value of the Cookie argument passed by ISwAddin::ConnectToSW

*CallbackFunction*
:   Function called when user clicks the context-sensitive menu icon (**see Remarks**)

*CallbackUpdateFunction*
:   Optional function that controls the state of the icon; if specified, then SOLIDWORKS calls this function before displaying the icon

    | If CallbackUpdateFunction returns... | Then SOLIDWORKS... |
    | --- | --- |
    | 0 | Deselects and disables the item |
    | 1 | Deselects and enables the item; this is the default state if no update function is specified |
    | 4 | Hides the item |

    (see **Remarks**)

*CustomNames*
:   Names of custom feature types (see **Remarks**)

*BitmapFilePath*
:   Path and file name of the bitmap for the context-sensitive menu icon

#### Return Value

True if the context-sensitive menu icon is added, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Frame::AddMenuPopupIcon2.

# ![](dotnetimages/collapse.gif)Example

[Add Shortcut Menus to Add-ins (C#)](Add_Shortcut_Menus_to_Add-ins_CSharp.htm)

[Add Shortcut Menus to Add-ins (VB.NET)](Add_Shortcut_Menus_to_Add-ins_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

See Add-in Callback and Enable Methods to learn how to specify CallbackFunction and CallbackUpdateFunction.

When the icon is clicked, the function specified in CallbackFunction can perform actions such as [displaying a third-party pop-up menu](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~ShowThirdPartyPopupMenu.html).

CustomNames is a semi-colon separated list of the names of the custom feature types. This argument is applicable only if SelectType is a custom feature type (like swSelATTRIBUTES); in the case of swSelATTRIBUTES, set this field to the name of the attribute definition.

# ![](dotnetimages/collapse.gif)See Also

####

[IFrame Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame.html)

[IFrame Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame_members.html)

[IFrame::AddMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenu.html)

[IFrame::AddMenuItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuItem2.html)

[IFrame::AddMenuPopupItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuPopupItem2.html)

[IFrame::GetMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~GetMenu.html)

[IFrame::GetMenux64 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~GetMenux64.html)

[IFrame::GetSubMenuCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~GetSubMenuCount.html)

[IFrame::GetSubMenus Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~GetSubMenus.html)

[IFrame::IGetSubMenus Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~IGetSubMenus.html)

[IFrame::RemoveMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~RemoveMenu.html)

[IFrame::RemoveMenuPopupIcon Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~RemoveMenuPopupIcon.html)

[IFrame::RenameMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~RenameMenu.html)

[IFrame::MenuPinned Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~MenuPinned.html)

[IFrame::AddMenuPopupIcon Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuPopupIcon.html)

[ISldWorks::AddItemToThirdPartyPopupMenu2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddItemToThirdPartyPopupMenu2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0