<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetProgressPos.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetProgressPos Method (IEdmTaskInstance) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskInstance Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html) : SetProgressPos Method (IEdmTaskInstance) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lPos*
:   Current position of the progress bar

*bsDocStr*
:   Description of what the add-in is currently doing

Updates the task list progress bar during execution of this task instance.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetProgressPos( _    ByVal lPos As System.Integer, _    ByVal bsDocStr As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetProgressPos(     System.int lPos,    System.string bsDocStr ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetProgressPos(  &   System.int lPos, &   System.String^ bsDocStr ) ``` | |

#### Parameters

*lPos*
:   Current position of the progress bar

*bsDocStr*
:   Description of what the add-in is currently doing

# ![](dotnetimages/collapse.gif)Example

See the examples in [IEdmTaskInstance](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html).

# ![](dotnetimages/collapse.gif)Remarks

The task add-in calls this method periodically during processing of the hook, [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd.TaskRun, to update the progress bar in the task list window of the PDM Administration tool.

Initialize the task list progress bar by calling [IEdmTaskinstance::SetProgressRange](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetProgressRange.html) at the start of processing of the hook, EdmCmdType.EdmCmd.TaskRun.

lPos is between 0 and lMax of IEdmTaskinstance::SetProgressRange.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskInstance Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html)

[IEdmTaskInstance Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010