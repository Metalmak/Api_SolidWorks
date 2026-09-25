<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~GetVar.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetVar Method (IEdmTaskInstance) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskInstance Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html) : GetVar Method (IEdmTaskInstance) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oVarIDorName*
:   ID or name of the card variable for which to get a value

Gets the value of a card variable created in the administration tool.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetVar( _    ByVal oVarIDorName As System.Object _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetVar(     System.object oVarIDorName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetVar(  &   System.Object^ oVarIDorName ) ``` | |

#### Parameters

*oVarIDorName*
:   ID or name of the card variable for which to get a value

#### Return Value

Value of a card variable

# ![](dotnetimages/collapse.gif)Remarks

The task add-in calls this method while the task is running on the server (EdmCmdType.EdmCmd\_TaskRun) to retrieve a variable value set by the add-in when it calls:

* [IEdmTaskInstance::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetVar.html) during the processing of the [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskLaunch hook when the user enters values on the data card displayed when the task is launched on the client computer.* [IEdmTaskProperties.SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetVar.html) during the processing of the EdmCmdType.EdmCmd\_TaskSetup hook when the user enters data card variable values on the task setup page.

Card variables accessible by this method must be created using the administration tool card editor and are not related to the user-defined variables accessed by [IEdmTaskInstance::GetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~GetValEx.html) and [IEdmTaskInstance::SetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetValEx.html).

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskInstance Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html)

[IEdmTaskInstance Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance_members.html)

[IEdmTaskInstance::SetVar Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetVar.html)

[Task Add-in Sample](TaskSample.htm)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010