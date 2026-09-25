<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetVar.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetVar Method (IEdmTaskProperties) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html) : GetVar Method (IEdmTaskProperties) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lVarID*
:   ID of variable for which to get a value

Gets the value of a card variable created in the administration tool and set by [IEdmTaskProperties::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetVar.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetVar( _    ByVal lVarID As System.Integer _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetVar(     System.int lVarID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetVar(  &   System.int lVarID ) ``` | |

#### Parameters

*lVarID*
:   ID of variable for which to get a value

#### Return Value

Value of a card variable

# ![](dotnetimages/collapse.gif)Remarks

The task add-in calls this method to retrieve a data card variable value that is set by the user on the task details page on the client computer. To save and retrieve the variable, the add-in calls [IEdmTaskProperties::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetVar.html) and this method, respectively, during the processing of the [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskSetup hook.

These data card variable values can also be retrieved when the task is executed on the server by calling [IEdmTaskInstance::GetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~GetVar.html).

Card variables accessible by this method must be created using the administration tool card editor and are not related to the user-defined variables accessed by [IEdmTaskProperties::GetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetValEx.html) and [IEdmTaskProperties::SetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetValEx.html).

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html)

[IEdmTaskProperties Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties_members.html)

[Task Add-in Sample](TaskSample.htm)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010