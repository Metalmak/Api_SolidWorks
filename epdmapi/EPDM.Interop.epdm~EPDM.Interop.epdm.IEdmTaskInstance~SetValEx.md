<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetValEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetValEx Method (IEdmTaskInstance) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskInstance Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html) : SetValEx Method (IEdmTaskInstance) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsValName*
:   User-defined variable name

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
:   User-defined variable name

*oValue*
:   Value of user-defined variable (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

This method can be called to set the value when the task is launched on the client computer ([EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_TaskLaunch) and [IEdmTaskInstance::GetValEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~GetValEx.html) can be called to get the value when the task is executed on the server (EdmCmdType.EdmCmd\_TaskRun).

Custom data types and objects must be serialized to a string, numeric type, or date before calling IEdmTaskInstance::SetValEx. For example:

1. Serialize the object data to XML or JSON using StringBuilder, XmlWriter, XmlSerializer, etc.- Call IEdmTaskInstance::SetValEx to store the resulting string.- Call IEdmTaskInstance::GetValEx to retrieve the stored string.- Initialize the new instance of the object from XML/JSON using StringReader, XmlReader, XmlSerializer, etc.

**NOTE**: The difference between this method and [IEdmTaskInstance::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance~SetVar.html) is that the latter requires a pre-defined card variable in the vault, whereas this method does not.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskInstance Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance.html)

[IEdmTaskInstance Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskInstance_members.html)

[Task Add-in Sample](TaskSample.htm)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010