<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.CreateMenuFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateMenuFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : CreateMenuFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of menu used in calls to [IEdmVault5::CreatePluginMenu](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~CreatePluginMenu.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum CreateMenuFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum CreateMenuFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class CreateMenuFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Cmf\_AddMenuIcons** | 32 = Adds toolbar button bitmaps to the menu |
| **Cmf\_AllItemsInSameFolder** | 1 = All of the selected files and folders are located in the same parent folder |
| **Cmf\_ContextMenu** | 8 = Context-sensitive menu; not a standard popup menu |
| **Cmf\_ContextMenuItem** | 64 = Context-sensitive menu for an item |
| **Cmf\_ContextMenuItemFolder** | 128 = Context-sensitive menu for an item folder |
| **Cmf\_DisableAddInReload** | 16 = Prevent SOLIDWORKS PDM Professional from querying the database to check whether updates have been made to the number of installed add-ins; this can be used to optimize the execution when called several times in a row |
| **Cmf\_GrayOutInvalidItems** | 4 = Disable menu items that are not currently applicable |
| **Cmf\_IncludeAdminReactors** | 2 = Include the [Administrate Add-ins](AdminDlg.htm) command |
| **Cmf\_ItemToolsMenu** | 256 = **Tools > Item** menu in the Item Explorer |
| **Cmf\_MenuBarAction** | 512 = **Actions** menu in the File Explorer |
| **Cmf\_MenuBarDisplay** | 2048 = **Display** menu in File Explorer |
| **Cmf\_MenuBarModify** | 1024 = **Modify** menu in File Explorer |
| **Cmf\_MenuBarTools** | 4096 = **Tools** menu in File Explorer |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)