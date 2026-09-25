<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRightFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmRightFlags Enumeration | |
| [See Also](#seealsobookmark)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRightFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags used in calls to [IEdmFolder5::HasRights](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~HasRights.html) and [IEdmFolder5::HasRightsEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~HasRightsEx.html) to check user rights. [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmRightFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmRightFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmRightFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmRight\_Add** | 8 = Permission to add files |
| **EdmRight\_AddFolder** | 16777216 = Permission to create subfolders |
| **EdmRight\_All** | -1 or 0xffffffff = Complete set of rights  **NOTE**: Do not use this constant in rights checking, because more flags might be added in the future. Instead, explicitly specify the rights bits. |
| **EdmRight\_BomActivate** | 1024 = Activate computed BOM |
| **EdmRight\_ChangeCard** | 65536 = Permission to change the contents of a file/folder data card |
| **EdmRight\_ColdStoreRestore** | 524288 = Restore file from cold storage |
| **EdmRight\_Delete** | 4 = Permission to delete files |
| **EdmRight\_DeleteFolder** | 64 = Permission to delete subfolders |
| **EdmRight\_DestroyTrash** | 256 = Destroy |
| **EdmRight\_EditFolderCard** | 512 = Edit folder card data |
| **EdmRight\_EditVerFreeVarData** | 1048576 = Edit version free variable data |
| **EdmRight\_IncrementRevision** | 32 = Permission to increment revision on files |
| **EdmRight\_Lock** | 2 = Permission to check out files |
| **EdmRight\_MandatoryVersionComments** | 67108864 = Must enter revision comments |
| **EdmRight\_MaySeeComputedBOM** | 2048 = See computed BOM |
| **EdmRight\_MoveFile** | 2097152 = Permission to move files |
| **EdmRight\_MoveFolder** | 8388608 = Permission to move folders |
| **EdmRight\_None** | 0 = No rights at all; used internally |
| **EdmRight\_OverwriteLatestVersion** | 33554432 = Overwrite latest version |
| **EdmRight\_PrivateState** | 4194304 = Permission to make state private |
| **EdmRight\_Read** | 1 = Permission to read files |
| **EdmRight\_RecoverTrash** | 128 = Recover files from the recycle bin |
| **EdmRight\_Rename** | 8 = Permission to rename files |
| **EdmRight\_RenameFolder** | 16777216 = Permission to rename folders |
| **EdmRight\_Rollback** | 262144 = Can run the rollback command in the history dialog box |
| **EdmRight\_Share** | 16 = Permission to share files |
| **EdmRight\_ShowWorkingVersion** | 131072 = Permission to see working versions, not just revisions |

# ![](dotnetimages/collapse.gif)Example

[Get and Set Folder Permissions (VB.NET)](Get_and_Set_Folder_Permissions_Example_VBNET.htm)

[Get and Set Folder Permissions (C#)](Get_and_Set_Folder_Permissions_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)