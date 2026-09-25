<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetVar.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetVar Method (IEdmTaskProperties) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html) : SetVar Method (IEdmTaskProperties) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lVarID*
:   ID of the variable for which to set a value (see **Remarks**)

*oValue*
:   Value to set

Sets the value of a card variable created in the administration tool.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetVar( _    ByVal lVarID As System.Integer, _    ByVal oValue As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetVar(     System.int lVarID,    System.object oValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetVar(  &   System.int lVarID, &   System.Object^ oValue ) ``` | |

#### Parameters

*lVarID*
:   ID of the variable for which to set a value (see **Remarks**)

*oValue*
:   Value to set

# ![](dotnetimages/collapse.gif)Remarks

The task add-in can display a data card with variable values that the user can modify when the task is launched on the client computer ([EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskLaunch). The add-in can call this method to store the variable values entered by the user.

The card variable value set by this method can be retrieved by calling:

* [IEdmTaskProperties::GetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetVar.html).* [IEdmTaskInstance::GetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~GetVar.html) during the processing of the EdmCmdType.EdmCmd\_TaskRun hook on the server where the task instance is running.

Card variables are created using the administration tool card editor and are not related to the user-defined variables accessed by [IEdmTaskInstance::GetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~GetValEx.html) and [IEdmTaskInstance::SetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetValEx.html).

The difference between this method and IEdmTaskInstance::SetValEx is that the latter does not require a pre-defined card variable in the vault, whereas this method does.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html)

[IEdmTaskProperties Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties_members.html)

[Task Add-in Sample](TaskSample.htm)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010