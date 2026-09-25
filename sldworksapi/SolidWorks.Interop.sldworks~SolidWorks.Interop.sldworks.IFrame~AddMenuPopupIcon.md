<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuPopupIcon.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddMenuPopupIcon Method (IFrame) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFrame Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame.html) : AddMenuPopupIcon Method (IFrame) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DocType*
:   Document type to which to add the context-sensitive menu icon

*SelectType*
:   Selection type to which to add the context-sensitive menu icon

*HintString*
:   Text displayed in the SOLIDWORKS status bar when the user moves the mouse over the icon

*CallbackFcnAndModule*
:   Function called when user clicks the context-sensitive menu icon (see **Remarks**)

*CustomNames*
:   Names of custom feature types (see **Remarks**)

*BitmapFilePath*
:   Path and file name of the bitmap for the context-sensitive menu icon

Adds an icon to a context-sensitive menu of a C++ SOLIDWORKS add-in.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddMenuPopupIcon( _    ByVal DocType As System.Integer, _    ByVal SelectType As System.Integer, _    ByVal HintString As System.String, _    ByVal CallbackFcnAndModule As System.String, _    ByVal CustomNames As System.String, _    ByVal BitmapFilePath As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFrame Dim DocType As System.Integer Dim SelectType As System.Integer Dim HintString As System.String Dim CallbackFcnAndModule As System.String Dim CustomNames As System.String Dim BitmapFilePath As System.String Dim value As System.Boolean   value = instance.AddMenuPopupIcon(DocType, SelectType, HintString, CallbackFcnAndModule, CustomNames, BitmapFilePath) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddMenuPopupIcon(     System.int DocType,    System.int SelectType,    System.string HintString,    System.string CallbackFcnAndModule,    System.string CustomNames,    System.string BitmapFilePath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddMenuPopupIcon(  &   System.int DocType, &   System.int SelectType, &   System.String^ HintString, &   System.String^ CallbackFcnAndModule, &   System.String^ CustomNames, &   System.String^ BitmapFilePath ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DocType*
:   Document type to which to add the context-sensitive menu icon

*SelectType*
:   Selection type to which to add the context-sensitive menu icon

*HintString*
:   Text displayed in the SOLIDWORKS status bar when the user moves the mouse over the icon

*CallbackFcnAndModule*
:   Function called when user clicks the context-sensitive menu icon (see **Remarks**)

*CustomNames*
:   Names of custom feature types (see **Remarks**)

*BitmapFilePath*
:   Path and file name of the bitmap for the context-sensitive menu icon

#### Return Value

True if the context-sensitive menu icon is added, false if not

# ![](dotnetimages/collapse.gif)Example

| C++ | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` //Add a single icon to the standard //SOLIDWORKS face context menu. swFrame->AddMenuPopupIcon( swDocPART, swSelFACES, CComBSTR(_T("UserPopupMenus.dll@MinibarItem1_Menu1_Callback,Facehintstring")), CComBSTR(_T("UserPopupMenus.dll@MinibarItem1_Menu1_Callback")), CComBSTR(_T("")), UserItem1_Menu1_bitmapFile, &iconSuccess ); ``` | |

# ![](dotnetimages/collapse.gif)Remarks

This method is supported in C++ applications only, and it only works for C++ applications implemented as **.dll** files, not as **.exe** files. Any function exposed as a callback from an context-sensitive menu icon must be declared as an EXPORT or included in your **.def** file.

The CallbackFcnAndModule argument specifies which function to call when the shortcut menu icon is clicked by the user. The syntax is as follows:

dllname@function

where:

|  |  |
| --- | --- |
| dllname | Name of your library as specified in the project **.def** file. The actual file name and the definition in the **.def** file must be the same. |
| function | Name of the function that gets called when the user clicks the icon. This function must also be declared as an EXPORT in your **.def** file.  See Add-in Callback and Enable Methods to learn how to implement your callback function. |

CustomNames is a semi-colon separated list of the names of the custom feature types. This argument is applicable only if SelectType is a custom feature type (like swSelATTRIBUTES); in the case of swSelATTRIBUTES, set this field to the name of the attribute definition.

# ![](dotnetimages/collapse.gif)See Also

####

[IFrame Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame.html)

[IFrame Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame_members.html)

[IFrame::RemoveMenuPopupIcon Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~RemoveMenuPopupIcon.html)

[IFrame::AddMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenu.html)

[IFrame::AddMenuItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuItem2.html)

[IFrame::GetMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~GetMenu.html)

[IFrame::GetSubMenuCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~GetSubMenuCount.html)

[IFrame::GetSubMenus Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~GetSubMenus.html)

[IFrame::RenameMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~RenameMenu.html)

[IFrame::AddMenuPopupItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuPopupItem2.html)

[IFrame::AddMenuPopupIcon2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuPopupIcon2.html)

[ISldWorks::AddItemToThirdPartyPopupMenu Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddItemToThirdPartyPopupMenu.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0