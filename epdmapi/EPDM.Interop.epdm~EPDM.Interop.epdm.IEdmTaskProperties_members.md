<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmTaskProperties Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmTaskProperties Interface |

The following tables list the members exposed by [IEdmTaskProperties](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [AddInName](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~AddInName.html) | Gets the name of the add-in that is used to execute this task. |
| ![ Property](dotnetimages/Property.gif) | [FormName](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~FormName.html) | Gets the name of the data card to show when the task is launched. |
| ![ Property](dotnetimages/Property.gif) | [IsScheduled](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~IsScheduled.html) | Gets whether this task is scheduled. |
| ![ Property](dotnetimages/Property.gif) | [RetryCount](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~RetryCount.html) | Gets the number of times to retry the task on failure. |
| ![ Property](dotnetimages/Property.gif) | [TaskFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~TaskFlags.html) | Gets or sets task-specific options. |
| ![ Property](dotnetimages/Property.gif) | [TaskGUID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~TaskGUID.html) | Gets the unique ID of this task definition. |
| ![ Property](dotnetimages/Property.gif) | [TaskID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~TaskID.html) | Gets the database ID of this task definition. |
| ![ Property](dotnetimages/Property.gif) | [TaskName](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~TaskName.html) | Gets the name of this task. |
| ![ Property](dotnetimages/Property.gif) | [TimeoutInSeconds](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~TimeoutInSeconds.html) | Gets the number of seconds to wait until failing the task. |
| ![ Property](dotnetimages/Property.gif) | [UserName](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~UserName.html) | Gets the name of the user as whom to execute this task. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetMenuCmds](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetMenuCmds.html) | Gets the menu commands set with [IEdmTaskProperties::SetMenuCmds](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetMenuCmds.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSel](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetSel.html) | Gets the selection of objects on which to execute this task. |
| ![ Method](dotnetimages/Method.gif) | [GetSetupPages](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetSetupPages.html) | Gets the setup pages added to the task property dialog box using [IEdmTaskProperties::SetSetupPages](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetSetupPages.html). |
| ![ Method](dotnetimages/Method.gif) | [GetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetValEx.html) | Gets the value of a user-defined variable created with [IEdmTaskProperties::SetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetValEx.html). |
| ![ Method](dotnetimages/Method.gif) | [GetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetVar.html) | Gets the value of a card variable created in the administration tool and set by [IEdmTaskProperties::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetVar.html). |
| ![ Method](dotnetimages/Method.gif) | [SetMenuCmds](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetMenuCmds.html) | Adds the specified menu commands to File Explorer context menus. |
| ![ Method](dotnetimages/Method.gif) | [SetSel](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetSel.html) | Sets the selection of objects on which to execute this task. |
| ![ Method](dotnetimages/Method.gif) | [SetSetupPages](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetSetupPages.html) | Adds setup pages to the task property dialog box for this task definition. |
| ![ Method](dotnetimages/Method.gif) | [SetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetValEx.html) | Sets a value for the specified user-defined variable. |
| ![ Method](dotnetimages/Method.gif) | [SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetVar.html) | Sets the value of a card variable created in the administration tool. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[Task Add-in Sample](TaskSample.htm)

[Standard Task Add-in](StandardTaskAddIn.htm)

[IEdmTaskMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskMgr.html)