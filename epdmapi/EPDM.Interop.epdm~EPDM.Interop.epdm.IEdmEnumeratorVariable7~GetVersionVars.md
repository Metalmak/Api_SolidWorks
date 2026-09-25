<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7~GetVersionVars.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetVersionVars Method (IEdmEnumeratorVariable7) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVariable7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7.html) : GetVersionVars Method (IEdmEnumeratorVariable7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oVersion*
:   Version number of variables to get; 0 to get the latest version

*lFolderID*
:   ID of the file's parent folder; 0 if the file is not shared

*ppoRetVariables*
:   Array of [IEdmVariableValue6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue6.html) interfaces; one interface for each variable value

*ppoRetConfigs*
:   Array of configuration or layout names

*poRetData*
:   [EdmGetVarData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData.html); extra information about the file

Gets the values of variables of the specified version directly from the database.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetVersionVars( _    ByVal oVersion As System.Object, _    ByVal lFolderID As System.Integer, _    ByRef ppoRetVariables() As System.Object, _    ByRef ppoRetConfigs() As System.String, _    ByRef poRetData As EdmGetVarData _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetVersionVars(     System.object oVersion,    System.int lFolderID,    out System.object[] ppoRetVariables,    out System.string[] ppoRetConfigs,    out EdmGetVarData poRetData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetVersionVars(  &   System.Object^ oVersion, &   System.int lFolderID, &   [Out] System.array<Object^>^ ppoRetVariables, &   [Out] System.array<String^>^ ppoRetConfigs, &   [Out] EdmGetVarData poRetData ) ``` | |

#### Parameters

*oVersion*
:   Version number of variables to get; 0 to get the latest version

*lFolderID*
:   ID of the file's parent folder; 0 if the file is not shared

*ppoRetVariables*
:   Array of [IEdmVariableValue6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue6.html) interfaces; one interface for each variable value

*ppoRetConfigs*
:   Array of configuration or layout names

*poRetData*
:   [EdmGetVarData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetVarData.html); extra information about the file

# ![](dotnetimages/collapse.gif)Example

[Get File Variable Data (VB.NET)](Get_File_Variable_Data_Example_VBNET.htm)

[Get File Variable Data (C#)](Get_File_Variable_Data_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

In previous versions of the API, you had to call [IEdmFile5::GetFileCopy](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetFileCopy.html) get a local copy of a file and then call [IEdmFile5::GetEnumeratorVariable](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetEnumeratorVariable.html) to read variables. This method is more efficient, because it retrieves the variable values directly from the database, removing the need to retrieve the file first.

When retrieving several variables, it is more efficient to use this method instead of multiple calls to [IEdmEnumeratorVariable5::GetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5~GetVar.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVariable7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7.html)

[IEdmEnumeratorVariable7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4