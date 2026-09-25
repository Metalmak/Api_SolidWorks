<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetSel.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetSel Method (IEdmTaskProperties) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html) : SetSel Method (IEdmTaskProperties) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poSel*
:   Array of [EdmTaskSel](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSel.html) structures; one structure for each selected object

Sets the selection of objects on which to execute this task.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetSel( _    ByVal poSel() As EdmTaskSel _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetSel(     EdmTaskSel[] poSel ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetSel(  &   array<EdmTaskSel>^ poSel ) ``` | |

#### Parameters

*poSel*
:   Array of [EdmTaskSel](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSel.html) structures; one structure for each selected object

# ![](dotnetimages/collapse.gif)Remarks

The user can select the objects on which the task performs from a dialog box that is displayed when the task add-in calls [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html). The hook, [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskLaunch, must be previously registered by calling [IEdmCmdMgr5::AddHook](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddHook.html) in your implementation of [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html). The add-in returns the user's selections in the [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html) structures that are returned by IEdmAddIn5::OnCmd.

You can set a selection of objects that should always be passed to the task instances by calling this method.

Call [IEdmTaskProperties::GetSel](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetSel.html) to get the objects set by this method.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html)

[IEdmTaskProperties Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties_members.html)

[Task Add-in Sample](TaskSample.htm)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010