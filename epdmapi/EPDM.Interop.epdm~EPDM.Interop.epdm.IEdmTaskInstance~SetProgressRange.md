<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetProgressRange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetProgressRange Method (IEdmTaskInstance) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskInstance Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html) : SetProgressRange Method (IEdmTaskInstance) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lMax*
:   Maximum position in the progress bar

*lPos*
:   0 <= Current position in the progress bar <= lMax

*bsDocStr*
:   Description of what the add-in is currently doing

Sets the range of the progress bar for the execution of this task instance.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetProgressRange( _    ByVal lMax As System.Integer, _    ByVal lPos As System.Integer, _    ByVal bsDocStr As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetProgressRange(     System.int lMax,    System.int lPos,    System.string bsDocStr ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetProgressRange(  &   System.int lMax, &   System.int lPos, &   System.String^ bsDocStr ) ``` | |

#### Parameters

*lMax*
:   Maximum position in the progress bar

*lPos*
:   0 <= Current position in the progress bar <= lMax

*bsDocStr*
:   Description of what the add-in is currently doing

# ![](dotnetimages/collapse.gif)Example

See the examples in [IEdmTaskInstance](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html).

# ![](dotnetimages/collapse.gif)Remarks

The task add-in calls this method at the start of processing of the hook, [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd.TaskRun, to initialize the task list progress bar in the task list window of the PDM Administration tool.

The task add-in calls [IEdmTaskInstance::SetProgressPos](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetProgressPos.html) periodically during processing of the hook, EdmCmdType.EdmCmd.TaskRun, to update the progress bar.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskInstance Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html)

[IEdmTaskInstance Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010