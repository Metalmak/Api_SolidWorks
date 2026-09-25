<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5~OnMenuItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| OnMenuItem Method (IEdmMenu5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmMenu5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html) : OnMenuItem Method (IEdmMenu5) |

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
:   ID of the currently active folder

*poSelFiles*
:   [List of selected files](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html)

*poSelFolders*
:   [List of selected folders](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html)

Obsolete. Superseded by [IEdmMenu7::OnMenuItem2.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu7~OnMenuItem2.html)

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function OnMenuItem( _    ByVal lItemID As System.Integer, _    ByVal lParentWnd As System.Integer, _    ByVal lCurrentFolderID As System.Integer, _    ByVal poSelFiles As EdmSelectionList5, _    ByVal poSelFolders As EdmSelectionList5 _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int OnMenuItem(     System.int lItemID,    System.int lParentWnd,    System.int lCurrentFolderID,    EdmSelectionList5 poSelFiles,    EdmSelectionList5 poSelFolders ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int OnMenuItem(  &   System.int lItemID, &   System.int lParentWnd, &   System.int lCurrentFolderID, &   EdmSelectionList5^ poSelFiles, &   EdmSelectionList5^ poSelFolders ) ``` | |

#### Parameters

*lItemID*
:   ID of the selected menu item

*lParentWnd*
:   Parent window handle (HWND)

*lCurrentFolderID*
:   ID of the currently active folder

*poSelFiles*
:   [List of selected files](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html)

*poSelFolders*
:   [List of selected folders](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html)

#### Return Value

User-interface elements that should be refreshed as defined in [EdmRefreshFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefreshFlag.html)

# ![](dotnetimages/collapse.gif)Remarks

You should call this method when a user selects a menu item belonging to this menu.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE:  Menu item does not belong to this menu.* S\_EDM\_MENU\_ITEM\_NOT\_APPLICABLE: The current selection of files and folders do not satisfy the constraints set by the command author. See [EdmMenuFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMenuFlags.html) sent to [IEdmCmdMgr5::AddCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddCmd.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmMenu5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html)

[IEdmMenu5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional