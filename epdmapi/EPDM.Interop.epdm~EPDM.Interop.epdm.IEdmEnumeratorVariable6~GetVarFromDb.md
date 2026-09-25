<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable6~GetVarFromDb.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetVarFromDb Method (IEdmEnumeratorVariable6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVariable6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable6.html) : GetVarFromDb Method (IEdmEnumeratorVariable6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsVarName*
:   Name of variable to read

*bsCfgName*
:   Name of configuration or layout from which to get the variable value; empty string for folders and file types that do not support configurations

*poRetValue*
:   Variable value

Reads a variable from the SOLIDWORKS PDM Professional database.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetVarFromDb( _    ByVal bsVarName As System.String, _    ByVal bsCfgName As System.String, _    ByRef poRetValue As System.Object _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetVarFromDb(     System.string bsVarName,    System.string bsCfgName,    out System.object poRetValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetVarFromDb(  &   System.String^ bsVarName, &   System.String^ bsCfgName, &   [Out] System.Object^ poRetValue ) ``` | |

#### Parameters

*bsVarName*
:   Name of variable to read

*bsCfgName*
:   Name of configuration or layout from which to get the variable value; empty string for folders and file types that do not support configurations

*poRetValue*
:   Variable value

#### Return Value

True if a variable is found, false if not

# ![](dotnetimages/collapse.gif)Remarks

To read a variable from a checked out file, call [IEdmEnumeratorVariable5::GetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5~GetVar.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: The variable is not found.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVariable6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable6.html)

[IEdmEnumeratorVariable6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0