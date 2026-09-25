<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmCmdType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmCmdType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Reasons for SOLIDWORKS PDM Professional to call [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmCmdType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmCmdType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmCmdType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmCmd\_ActivateAPITab** | 57 = Custom vault view tab is selected in File Explorer; sent only to add-ins that created a vault view tab in File Explorer |
| **EdmCmd\_CardButton** | 37 = The user clicked either **OK** or a button whose command is enclosed in brackets ("<...>") in the file data card |
| **EdmCmd\_CardInput** | 38 = The user modified a value in a file or folder data card |
| **EdmCmd\_CardListSrc** | 39 = The add-in should provide a list that is used in a card |
| **EdmCmd\_DeSelectItem** | 56 = Item is deselected File Explorer; sent only to add-ins that created a vault view tab in File Explorer |
| **EdmCmd\_InstallAddIn** | 23 = The add-in is being installed |
| **EdmCmd\_Menu** | 1 = User clicked a menu command or a toolbar button that was created by the add-in |
| **EdmCmd\_PostAdd** | 12 = One or more files were added to the file vault |
| **EdmCmd\_PostAddFolder** | 28 = One or more folders were added to the file vault |
| **EdmCmd\_PostCopy** | 20 = One or more files were copied to a new folder |
| **EdmCmd\_PostCopyFolder** | 36 = One or more folders were copied to a new parent folder |
| **EdmCmd\_PostDelete** | 14 = One or more files have been deleted |
| **EdmCmd\_PostDeleteFolder** | 30 = One or more folders were deleted from the file vault |
| **EdmCmd\_PostGet** | 26 = One or more files were copied from the archive to the local hard disk |
| **EdmCmd\_PostLabel** | 47 = A label has been created |
| **EdmCmd\_PostLabelAddItem** | 53 = A label has gotten a file or folder added to it |
| **EdmCmd\_PostLabelDelete** | 49 = A label has been deleted |
| **EdmCmd\_PostLabelModify** | 51 = A label has been renamed or gotten its comment updated |
| **EdmCmd\_PostLock** | 4 = One or more files have been checked out |
| **EdmCmd\_PostMove** | 22 = One or more files were moved to a new folder |
| **EdmCmd\_PostMoveFolder** | 34 = One or more folders were moved to a new parent folder |
| **EdmCmd\_PostRename** | 16 = One or more files were renamed |
| **EdmCmd\_PostRenameFolder** | 32 = One or more folders were renamed |
| **EdmCmd\_PostShare** | 18 = One or more files were shared to a new folder |
| **EdmCmd\_PostState** | 10 = One or more files had their states changed |
| **EdmCmd\_PostUndoLock** | 8 = One or more files had their locks removed without any changes sent to the file vault |
| **EdmCmd\_PostUnlock** | 6 = One or more files have been checked in |
| **EdmCmd\_PreAdd** | 11 = One or more files are about to be added to the file vault |
| **EdmCmd\_PreAddFolder** | 27 = One or more folders are about to be added to the file vault |
| **EdmCmd\_PreCopy** | 19 = One or more files are about to be copied to a new folder |
| **EdmCmd\_PreCopyFolder** | 35 = One or more folders are about to be copied to a new parent folder |
| **EdmCmd\_PreDelete** | 13 = One or more files are about to be deleted |
| **EdmCmd\_PreDeleteFolder** | 29 = One or more folders are about to be deleted from the file vault |
| **EdmCmd\_PreExploreInit** | 54 = A new instance of File Explorer is opening; handle this command in your add-in by calling [IEdmCmdMgf6::AddVaultViewTab](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr6~AddVaultViewTab.html) for each custom tab you want to add to the vault view in File Explorer |
| **EdmCmd\_PreGet** | 25 = One or more files are about to be copied from the archive to the local hard disk |
| **EdmCmd\_PreLabel** | 46 = A label is about to be created |
| **EdmCmd\_PreLabelAddItem** | 52 = A label is about to get a file or folder added to it |
| **EdmCmd\_PreLabelDelete** | 48 = A label is about to be deleted |
| **EdmCmd\_PreLabelModify** | 50 = A label is about to be renamed or get its comment updated |
| **EdmCmd\_PreLock** | 3 = One or more files are about to be checked out |
| **EdmCmd\_PreMove** | 21 = One or more files are about to be moved to a new folder |
| **EdmCmd\_PreMoveFolder** | 33 = One or more folders are about to be moved to a new parent folder |
| **EdmCmd\_PreRename** | 15 = One or more files are about to be renamed |
| **EdmCmd\_PreRenameFolder** | 31 = One or more folders are about to be renamed |
| **EdmCmd\_PreShare** | 17 = One or more files are about to be shared to a new folder |
| **EdmCmd\_PreState** | 9 = One or more files are about to have their states changed |
| **EdmCmd\_PreUndoLock** | 7 = One or more files are about to get their locks removed without any changes sent to the file vault |
| **EdmCmd\_PreUnlock** | 5 = One or more files are about to be checked in |
| **EdmCmd\_SelectItem** | 55 = Item is selected in File Explorer; sent only to add-ins that created a vault view tab in File Explorer |
| **EdmCmd\_SerialNo** | 2 = The add-in should generate a new serial number |
| **EdmCmd\_TaskDetails** | 42 = Use this hook to add your own custom page to the [task](Tasks.htm) details dialog box in the task list |
| **EdmCmd\_TaskLaunch** | 44 = The [task](Tasks.htm) is being launched; add your own user interface to permit user input |
| **EdmCmd\_TaskLaunchButton** | 45 = **OK** or **Cancel** was clicked in the [task](Tasks.htm) launch dialog box |
| **EdmCmd\_TaskRun** | 43 = This hook is called on the [task](Tasks.htm) server; you should perform the actual work there |
| **EdmCmd\_TaskSetup** | 40 = Use this hook to add a task setup page to a [task](Tasks.htm) properties dialog box wizard |
| **EdmCmd\_TaskSetupButton** | 41 = **OK** or **Cancel** was clicked in the [task](Tasks.htm) properties dialog box wizard |
| **EdmCmd\_UninstallAddIn** | 24 = The add-in is about to be uninstalled |
| **EdmCmd\_UserTabDelete** | 58 = Sent only to add-ins that created a vault view tab in File Explorer; called when File Explorer closes; opportunity for add-in to clean up tab-related items |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[EdmCmdData Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html)

[EdmCmd Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd.html)

[IEdmCmdMgr5::AddHook Method](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddHook.html)