<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetOpMsg.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmGetOpMsg Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGetOpMsg Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Log error messages; used in calls to [IEdmGetOpCallback::LogMessage](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~LogMessage.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmGetOpMsg     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmGetOpMsg : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmGetOpMsg : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Egom\_ErrorRunningPostAddins** | 3 = An error occurred running add-ins that implement hooks on [EdmCmd\_PostGet or EdmCmd\_PostLock](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html) commands |
| **Egom\_LockNotificationsError** | 1 = Error sending check-out notifications |
| **Egom\_Undefined** | 0 = Undefined message |
| **Egom\_UndoLockAfterErrorFailed** | 2 = The attempt to unlock a file after its check-out failed has failed |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)