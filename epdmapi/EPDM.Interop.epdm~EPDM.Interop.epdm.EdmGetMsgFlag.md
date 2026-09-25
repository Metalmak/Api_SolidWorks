<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetMsgFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmGetMsgFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGetMsgFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of message returned used in calls to [IEdmInbox5::GetFirstMessagePosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5~GetFirstMessagePosition.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmGetMsgFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmGetMsgFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmGetMsgFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmGetMsg\_Notifications** | 4 = Return only file or folder notifications |
| **EdmGetMsg\_OnlyNew** | 1 = Return only messages that have not been processed before |
| **EdmGetMsg\_OnlyUnread** | 8 = Return only messages having the [IEdmMessage5::IsRead](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMessage5~IsRead.html) flag set to true |
| **EdmGetMsg\_UserMessages** | 2 = Return only messages sent from users |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)