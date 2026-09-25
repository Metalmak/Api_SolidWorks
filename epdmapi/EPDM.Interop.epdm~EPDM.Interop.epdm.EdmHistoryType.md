<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmHistoryType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmHistoryType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmHistoryType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of history record; used by the [IEdmHistory](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory.html) interface. [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmHistoryType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmHistoryType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmHistoryType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmhist\_ColdStoreRestore** | 262144 = A file was restored from cold storage |
| **Edmhist\_FileBranch** | 4194304 |
| **Edmhist\_FileBranchMerge** | 8388608 |
| **Edmhist\_FileColdStore** | 1024 = A file was moved to the cold storage |
| **Edmhist\_FileDelete** | 16 = A file was deleted to the bit bucket |
| **Edmhist\_FileLabel** | 128 = A label was applied to a file |
| **Edmhist\_FileMove** | 4 = A file was moved |
| **Edmhist\_FileParallelState** | 61708864 |
| **Edmhist\_FilePendingState** | 33554432 |
| **Edmhist\_FileRename** | 2 = A file was renamed |
| **Edmhist\_FileRevision** | 512 = A revision was set on the file |
| **Edmhist\_FileRollback** | 8 = A file was rolled back |
| **Edmhist\_FileShare** | 1 = A file was shared |
| **Edmhist\_FileState** | 256 = The file’s workflow state was changed |
| **Edmhist\_FileUndelete** | 32 = A file was recovered from the bit bucket |
| **Edmhist\_FileUndoLock** | 2097152 |
| **Edmhist\_FileVerFreeVar** | 524288 = File version-free variables were updated |
| **Edmhist\_FileVersion** | 64 = A file was checked in, producing a new version |
| **Edmhist\_FileVersionOverwrite** | 16777216 |
| **Edmhist\_FolderCardData** | 131072 = A folder’s properties were edited |
| **Edmhist\_FolderCreate** | 8192 = A folder was created |
| **Edmhist\_FolderDelete** | 2048 = A folder was deleted to the bit bucket |
| **Edmhist\_FolderLabel** | 65536 = A label was applied to a folder |
| **Edmhist\_FolderMove** | 32768 = A folder was moved |
| **Edmhist\_FolderRename** | 16384 = A folder was renamed |
| **Edmhist\_FolderUndelete** | 4096 = A folder was recovered from the bit bucket |
| **Edmhist\_FolderVerFreeVar** | 1048576 = Folder version-free variables were updated |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)