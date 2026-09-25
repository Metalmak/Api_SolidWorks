<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5~GetUpdateVars.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetUpdateVars Method (IEdmEnumeratorVariable5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVariable5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5.html) : GetUpdateVars Method (IEdmEnumeratorVariable5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFolderID*
:   ID of the file's parent folder

*ppoRetVariables*
:   Array of [IEdmVariableValue5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue5.html); one interface for each variable value

Gets values for the variables that can be updated in this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetUpdateVars( _    ByVal lFolderID As System.Integer, _    ByRef ppoRetVariables() As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetUpdateVars(     System.int lFolderID,    out System.object[] ppoRetVariables ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetUpdateVars(  &   System.int lFolderID, &   [Out] System.array<Object^>^ ppoRetVariables ) ``` | |

#### Parameters

*lFolderID*
:   ID of the file's parent folder

*ppoRetVariables*
:   Array of [IEdmVariableValue5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue5.html); one interface for each variable value

# ![](dotnetimages/collapse.gif)Example

[Access File Card Variables (VB.NET)](Access_File_Card_Variables_Example_VBNET.htm)

[Access File Card Variables (C#)](Access_File_Card_Variables_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

C++ users must call SafeArrayDestroy to free the returned array elements.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_FILE\_NOT\_LOCKED\_BY\_YOU: The file is not checked out.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVariable5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5.html)

[IEdmEnumeratorVariable5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5_members.html)

[IEdmEnumeratorVariable5::StoreValuesFromDatabase Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5~StoreValuesFromDatabase.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2