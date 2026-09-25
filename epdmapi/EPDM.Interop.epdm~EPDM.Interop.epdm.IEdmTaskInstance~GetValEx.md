<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~GetValEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetValEx Method (IEdmTaskInstance) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskInstance Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html) : GetValEx Method (IEdmTaskInstance) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsValName*
:   Name of a user-defined variable

Gets the value of the specified user-defined variable.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetValEx( _    ByVal bsValName As System.String _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetValEx(     System.string bsValName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetValEx(  &   System.String^ bsValName ) ``` | |

#### Parameters

*bsValName*
:   Name of a user-defined variable

#### Return Value

Value of user-defined variable (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Create a Task that Finds Files in Workflow States (VB.NET)](Schedule_Task_to_Find_Files_in_State_Addin_Example_VBNET.htm)

[Create a Task that Finds Files in Workflow States (C#)](Schedule_Task_to_Find_Files_in_State_Addin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method gets the value of a user-defined variable that is created by [IEdmTaskInstance::SetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetValEx.html) or [IEdmTaskProperties::SetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetValEx.html). User-defined variables are usually created during the processing of the [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskLaunch or the EdmCmdType.EdmCmd\_TaskSetup hook and are usually read during the processing of the EdmCmdType.EdmCmd\_TaskRun hook.

Custom data types and objects must have been serialized to a string, numeric type, or date before calling IEdmTaskInstance::SetValEx or IEdmTaskProperites::SetValEx. For example:

1. Serialize the object data to XML or JSON using StringBuilder, XmlWriter, XmlSerializer, etc.- Call IEdmTaskInstance::SetValEx or IEdmTaskProperties::SetValEx to store the resulting string.- Call IEdmTaskInstance::GetValEx to retrieve the stored string.- Initialize the new instance of the object from XML/JSON using StringReader, XmlReader, XmlSerializer, etc.

**NOTE**: User-defined variables are not related to the card variables created using the administration tool. To access card variables, call [IEdmTaskInstance::GetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~GetVar.html) and [IEdmTaskInstance::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetVar.html).

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskInstance Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html)

[IEdmTaskInstance Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010