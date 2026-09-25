<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetValEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetValEx Method (IEdmTaskProperties) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html) : SetValEx Method (IEdmTaskProperties) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsValName*
:   Name of the user-defined variable for which to set a value

*oValue*
:   Value of user-defined variable (see **Remarks**)

Sets a value for the specified user-defined variable.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetValEx( _    ByVal bsValName As System.String, _    ByVal oValue As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetValEx(     System.string bsValName,    System.object oValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetValEx(  &   System.String^ bsValName, &   System.Object^ oValue ) ``` | |

#### Parameters

*bsValName*
:   Name of the user-defined variable for which to set a value

*oValue*
:   Value of user-defined variable (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Create a Task that Finds Files in Workflow States (VB.NET)](Schedule_Task_to_Find_Files_in_State_Addin_Example_VBNET.htm)

[Create a Task that Finds Files in Workflow States (C#)](Schedule_Task_to_Find_Files_in_State_Addin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call this method:

* to store variable data entered by the user in the task definition setup page on the client machine.* during the processing of the [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskSetup hook.

Custom data types and objects must be serialized to a string, numeric type, or date before calling this method. For example:

1. Serialize the object data to XML or JSON using StringBuilder, XmlWriter, XmlSerializer, etc.- Call IEdmTaskProperites::SetValEx to store the resulting string.- Call [IEdmTaskProperties::GetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetValEx.html) to retrieve the stored string.- Initialize the new instance of the object from XML/JSON using StringReader, XmlReader, XmlSerializer, etc.

To get the user-defined values when the task is executing on the server, call [IEdmTaskInstance::GetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~GetValEx.html) during the processing of the EdmCmdType.EdmCmd\_TaskRun hook.

**NOTE:** The difference between this method and [IEdmTaskProperties::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetVar.html) is that the latter requires a pre-defined card variable in the vault, whereas this method does not.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html)

[IEdmTaskProperties Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010