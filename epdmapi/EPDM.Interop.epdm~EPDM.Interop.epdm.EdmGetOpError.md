<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetOpError.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmGetOpError Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGetOpError Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Cold storage file retrieval error codes; used in calls to [IEdmGetOpCallback2::ReportFailureEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback2~ReportFailureEx.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmGetOpError     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmGetOpError : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmGetOpError : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmGetErr\_InColdStorageAvailable** | 1 = The version you are attempting to retrieve is in cold storage and needs to be retrieved from the backup media |
| **EdmGetErr\_InColdStorageDeleted** | 2 = The version you are attempting to retrieve was sent to cold storage and deleted |
| **EdmGetErr\_InColdStoragePermissionDenied** | 3 = The version you are attempting to retrieve is in cold storage, and you lack permission to restore it |
| **EdmGetErr\_InColdStorageRestoreFailed** | 4 = Could not retrieve the file from cold storage |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)