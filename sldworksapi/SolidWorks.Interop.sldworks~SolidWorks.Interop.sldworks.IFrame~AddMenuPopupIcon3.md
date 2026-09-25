<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuPopupIcon3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddMenuPopupIcon3 Method (IFrame) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFrame Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame.html) : AddMenuPopupIcon3 Method (IFrame) |

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

*ImageList*
:   Array of strings for the paths for the image files for the context-sensitive menu icon (see **Remarks**)

Adds an icon to a context-sensitive menu of a SOLIDWORKS add-in.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddMenuPopupIcon3( _    ByVal DocType As System.Integer, _    ByVal SelectType As System.Integer, _    ByVal HintString As System.String, _    ByVal Identifier As System.Integer, _    ByVal CallbackFunction As System.String, _    ByVal CallbackUpdateFunction As System.String, _    ByVal CustomNames As System.String, _    ByVal ImageList As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFrame Dim DocType As System.Integer Dim SelectType As System.Integer Dim HintString As System.String Dim Identifier As System.Integer Dim CallbackFunction As System.String Dim CallbackUpdateFunction As System.String Dim CustomNames As System.String Dim ImageList As System.Object Dim value As System.Boolean   value = instance.AddMenuPopupIcon3(DocType, SelectType, HintString, Identifier, CallbackFunction, CallbackUpdateFunction, CustomNames, ImageList) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddMenuPopupIcon3(     System.int DocType,    System.int SelectType,    System.string HintString,    System.int Identifier,    System.string CallbackFunction,    System.string CallbackUpdateFunction,    System.string CustomNames,    System.object ImageList ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddMenuPopupIcon3(  &   System.int DocType, &   System.int SelectType, &   System.String^ HintString, &   System.int Identifier, &   System.String^ CallbackFunction, &   System.String^ CallbackUpdateFunction, &   System.String^ CustomNames, &   System.Object^ ImageList ) ``` | |

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

*ImageList*
:   Array of strings for the paths for the image files for the context-sensitive menu icon (see **Remarks**)

#### Return Value

True if the context-sensitive menu icon is added, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Frame::AddMenuPopupIcon3.

# ![](dotnetimages/collapse.gif)Example

[Add Button to Context-sensitive Menu (C#)](Add_Button_to_Context-sensitive_Menu_Example_CSharp.htm)

[Add Button to Context-sensitive Menu (VB.NET)](Add_Button_to_Context-sensitive_Menu_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

See Add-in Callback and Enable Methods to learn how to specify CallbackFunction and CallbackUpdateFunction.

When the icon is clicked, the function specified in CallbackFunction can perform actions such as [displaying a third-party pop-up menu](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~ShowThirdPartyPopupMenu.html).

CustomNames is a semi-colon separated list of the names of the custom feature types. This argument is applicable only if SelectType is a custom feature type (like swSelATTRIBUTES); in the case of swSelATTRIBUTES, set this field to the name of the attribute definition.

This method supports scaling for high resolution screens with high resolution operating system scaling options.

ImageList images can be:

* 20 x 20 pixels* 32 x 32 pixels* 40 x 40 pixels* 64 x 64 pixels* 96 x 96 pixels* 128 x128 pixels

Images should use 256-color palette.

# ![](dotnetimages/collapse.gif)See Also

####

[IFrame Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame.html)

[IFrame Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame_members.html)

[IFrame::AddMenu Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenu.html)

[IFrame::AddMenuItem2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuItem2.html)

[IFrame::AddMenuPopupIcon Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuPopupIcon.html)

[IFrame::AddMenuPopupItem2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuPopupItem2.html)

[IFrame::GetMenu Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~GetMenu.html)

[IFrame::GetMenux64 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~GetMenux64.html)

[IFrame::GetSubMenuCount Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~GetSubMenuCount.html)

[IFrame::GetSubMenus Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~GetSubMenus.html)

[IFrame::IGetSubMenus Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~IGetSubMenus.html)

[IFrame::MenuPinned Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~MenuPinned.html)

[IFrame::RemoveMenu Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~RemoveMenu.html)

[IFrame::RemoveMenuPopupIcon Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~RemoveMenuPopupIcon.html)

[IFrame::RenameMenu Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~RenameMenu.html)

[IFrame::AddItemToThirdPartyPopupMenu2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddItemToThirdPartyPopupMenu2.html)

[ISldWorks::GetImageSize Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetImageSize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0