<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmTaskFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmTaskFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Task add-in flags used in [IEdmTaskProperties::TaskFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~TaskFlags.html) and [EdmTaskInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskInfo.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmTaskFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmTaskFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmTaskFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmTask\_Nothing** | 0 = None of the other flags |
| **EdmTask\_SupportsChangeState** | 16 = Task can be launched via a workflow, state, change command |
| **EdmTask\_SupportsDetails** | 4 = Add-in extends the task details dialog box in the task list window in the Administration tool; the add-in will receive a call to its [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html) method with the argument [EdmCmdType.EdmCmd\_TaskDetails](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmColType.html) when the dialog box is to be extended |
| **EdmTask\_SupportsInitExec** | 2 = Add-in wants to have its [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html) method called when the user launches the task; this callback type ([EdmCmdType.EdmCmd\_TaskLaunch](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html)) can be used to provide a more sophisticated user interface than one created with the card editor; if this flag is included, then multiple files will be processed by a single task instance; otherwise, each file will be processed by a separate task instance |
| **EdmTask\_SupportsInitForm** | 1 = Add-in supports displaying of a card created with the card editor; the card is used as the user interface when the task is launched, and the values of the card are accessible to the task add-in when it is executed |
| **EdmTask\_SupportsScheduling** | 8 = Task can be scheduled |

# ![](dotnetimages/collapse.gif)Remarks

The flags indicate what a task add-in is capable of doing.

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[Programming Tasks](Tasks.htm)