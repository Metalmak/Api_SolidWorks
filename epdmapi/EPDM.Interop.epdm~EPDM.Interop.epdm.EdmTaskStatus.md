<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskStatus.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmTaskStatus Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmTaskStatus Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Task add-in statuses.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmTaskStatus     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmTaskStatus : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmTaskStatus : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmTaskStat\_CancelPending** | 6 = **Cancel** clicked, but the host computer hasn't noticed it yet |
| **EdmTaskStat\_DoneCancelled** | 8 = Task terminated through canceling |
| **EdmTaskStat\_DoneFailed** | 9 = Task completed with errors |
| **EdmTaskStat\_DoneOK** | 7 = Task completed successfully |
| **EdmTaskStat\_ResumePending** | 11 = **Resume** clicked after task was suspended, but the host server hasn't noticed it yet |
| **EdmTaskStat\_Retrying** | 4 = Execution has failed at least once, but the framework is trying to execute the add-in again |
| **EdmTaskStat\_Running** | 3 = Task add-in is running on the host computer |
| **EdmTaskStat\_Starting** | 2 = Task starting on the host computer |
| **EdmTaskStat\_Suspended** | 5 = Task suspended by the user |
| **EdmTaskStat\_SuspensionPending** | 10 = **Suspend** clicked, but the task add-in hasn't noticed it yet |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmTaskInstance::GetStatus Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~GetStatus.html)

[IEdmTaskInstance::SetStatus Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetStatus.html)