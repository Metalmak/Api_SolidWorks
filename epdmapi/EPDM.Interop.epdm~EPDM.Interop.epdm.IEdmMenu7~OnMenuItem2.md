<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu7~OnMenuItem2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| OnMenuItem2 Method (IEdmMenu7) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmMenu7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu7.html) : OnMenuItem2 Method (IEdmMenu7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lItemID*
:   ID of the selected menu item

*lParentWnd*
:   Parent window handle (HWND)

*lCurrentFolderID*
:   ID of currently active folder

*poSelObjects*
:   [List of selected objects](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6.html) (files, folders, items, etc.)

Executes the command for the selected menu item.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function OnMenuItem2( _    ByVal lItemID As System.Integer, _    ByVal lParentWnd As System.Integer, _    ByVal lCurrentFolderID As System.Integer, _    ByVal poSelObjects As IEdmSelectionList6 _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int OnMenuItem2(     System.int lItemID,    System.int lParentWnd,    System.int lCurrentFolderID,    IEdmSelectionList6 poSelObjects ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int OnMenuItem2(  &   System.int lItemID, &   System.int lParentWnd, &   System.int lCurrentFolderID, &   IEdmSelectionList6^ poSelObjects ) ``` | |

#### Parameters

*lItemID*
:   ID of the selected menu item

*lParentWnd*
:   Parent window handle (HWND)

*lCurrentFolderID*
:   ID of currently active folder

*poSelObjects*
:   [List of selected objects](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6.html) (files, folders, items, etc.)

#### Return Value

User-interface elements that should be refreshed as defined in [EdmRefreshFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefreshFlag.html)

# ![](dotnetimages/collapse.gif)Example

[Display Menu of Commands (VB.NET)](Display_Menu_of_Commands_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

You should call this method when a user selects a menu item belonging to this menu.

**NOTE:** This method supersedes IEdmMenu5::OnMenuItem, which only works with files and folders. IEdmMenu7::OnMenuItem2 works with files and folders as well as other object types such as items.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: Menu item does not belong to this menu.* S\_EDM\_MENU\_ITEM\_NOT\_APPLICABLE: The current selection of objects do not satisfy the constraints set by the command author. See [EdmMenuFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMenuFlags.html) sent to [IEdmCmdMgr5::AddCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddCmd.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmMenu7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu7.html)

[IEdmMenu7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011