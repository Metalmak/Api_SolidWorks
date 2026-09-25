<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMenuFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmMenuFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmMenuFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags used by [IEdmCmdMgr5::AddCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddCmd.html) when writing an [add-in that supports menu commands](vbmenuitem.htm). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmMenuFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmMenuFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmMenuFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmMenu\_Administration** | 512 = The command is displayed in [SOLIDWORKS PDM Professional Administration](AddInAdminMenu.htm) tool instead of the File Explorer |
| **EdmMenu\_ContextMenuItem** | 1024 = The command is displayed in the file's context menu |
| **EdmMenu\_ContextMenuItemFolder** | 2048 = The command is displayed in the folder's context menu |
| **EdmMenu\_HastItemToolbarButton** | 8192 = The command has a button in the Item Explorer toolbar |
| **EdmMenu\_HasToolbarButton** | 128 = The command has a button in the File Explorer toolbar; see [IEdmCmdMgr5::AddToolbarImage](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddToolbarImage.html) |
| **EdmMenu\_ItemToolsMenu** | 4096 = The command is displayed in the Item Explorer tools menu |
| **EdmMenu\_MustHaveSelection** | 1 = The command is only available when the user has selected files or folders in the File Explorer file list |
| **EdmMenu\_NeverInContextMenu** | 64 = The command should not be present in the right-click, context menu, only in the File Explorer Tools menu |
| **EdmMenu\_Nothing** | 0 = Default behavior; no restrictions and no toolbar |
| **EdmMenu\_OnlyFiles** | 2 = The command is not available for selections containing folders, only for files |
| **EdmMenu\_OnlyFolders** | 4 = The command is not available for selections containing files, only for folders |
| **EdmMenu\_OnlyInContextMenu** | 32 = The command should only be present in the right-click, context menu, not in the File Explorer Tools menu |
| **EdmMenu\_OnlyMultipleSelection** | 16 = The command is only available for multiple selections, not for single files or folders |
| **EdmMenu\_OnlySingleSelection** | 8 = The command is only available if only one file or folder has been selected, not for multiple selections |
| **EdmMenu\_OwnerDrawToolbarButton** | 256 = The command uses custom drawing of its toolbar button by implementing [IEdmAddInDrawButton5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInDrawButton5.html) |
| **EdmMenu\_ShowInMenuBarAction** | 16384 = The command is displayed in the Action menu in the File Explorer toolbar |
| **EdmMenu\_ShowInMenuBarDisplay** | 65536 = The command is displayed in the Display menu in the File Explorer toolbar |
| **EdmMenu\_ShowInMenuBarModify** | 32768 = The command is displayed in the Modify menu in the File Explorer toolbar |
| **EdmMenu\_ShowInMenuBarTools** | 131072 = The command is displayed in the Tools menu in the File Explorer toolbar |

# ![](dotnetimages/collapse.gif)Remarks

The flags specify various properties for your command.

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)