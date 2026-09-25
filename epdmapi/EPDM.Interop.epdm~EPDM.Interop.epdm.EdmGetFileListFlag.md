<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetFileListFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmGetFileListFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGetFileListFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Files to return by [IEdmBatchGet::GetFileList](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet~GetFileList.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmGetFileListFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmGetFileListFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmGetFileListFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Egflf\_GetFailed** | 8 = Operation failed |
| **Egflf\_GetLocked** | 2 = Return files checked out by the operation |
| **Egflf\_GetRetrieved** | 1 = Return files retrieved by the operation |
| **Egflf\_GetUnprocessed** | 4 = Return files not processed by the operation |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)