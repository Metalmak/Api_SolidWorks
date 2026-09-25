<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetStatus.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetStatus Method (IEdmTaskInstance) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskInstance Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html) : SetStatus Method (IEdmTaskInstance) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eStatus*
:   Status of this task as defined in [EdmTaskStatus](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskStatus.html)

*lHRESULT*
:   Optional error code to display in the properties window when terminating the task; valid only if eStatus is EdmTaskStatus.EdmTaskStat\_DoneFailed

*bsCustomMsg*
:   Optional error message to display when terminating the task; valid only if eStatus is EdmTaskStatus.EdmTaskStat\_DoneFailed

*oNotificationAttachments*
:   Optional array of [EdmSelItem2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2.html) structures; one structure for each file link to add to the notification message that is sent when the task completes

*bsExtraNotificationMsg*
:   Optional message to append to the notification message that is sent when the task completes

Sets the specified status of this task instance.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetStatus( _    ByVal eStatus As EdmTaskStatus, _    Optional ByVal lHRESULT As System.Integer, _    Optional ByVal bsCustomMsg As System.String, _    Optional ByVal oNotificationAttachments As System.Object, _    Optional ByVal bsExtraNotificationMsg As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetStatus(     EdmTaskStatus eStatus,    System.int lHRESULT,    System.string bsCustomMsg,    System.object oNotificationAttachments,    System.string bsExtraNotificationMsg ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetStatus(  &   EdmTaskStatus eStatus, &   System.int lHRESULT, &   System.String^ bsCustomMsg, &   System.Object^ oNotificationAttachments, &   System.String^ bsExtraNotificationMsg ) ``` | |

#### Parameters

*eStatus*
:   Status of this task as defined in [EdmTaskStatus](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskStatus.html)

*lHRESULT*
:   Optional error code to display in the properties window when terminating the task; valid only if eStatus is EdmTaskStatus.EdmTaskStat\_DoneFailed

*bsCustomMsg*
:   Optional error message to display when terminating the task; valid only if eStatus is EdmTaskStatus.EdmTaskStat\_DoneFailed

*oNotificationAttachments*
:   Optional array of [EdmSelItem2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2.html) structures; one structure for each file link to add to the notification message that is sent when the task completes

*bsExtraNotificationMsg*
:   Optional message to append to the notification message that is sent when the task completes

# ![](dotnetimages/collapse.gif)Example

See the examples in [IEdmTaskInstance](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html).

# ![](dotnetimages/collapse.gif)Remarks

The task add-in calls this method to inform the framework about the current status of the task.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskInstance Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html)

[IEdmTaskInstance Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance_members.html)

[IEdmTaskInstance::GetStatus Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~GetStatus.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010