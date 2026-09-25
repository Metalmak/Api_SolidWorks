<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7~GenerateDefaultValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GenerateDefaultValues Method (IEdmEnumeratorVariable7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVariable7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7.html) : GenerateDefaultValues Method (IEdmEnumeratorVariable7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFolderID*
:   ID of the file's parent folder

*bWriteValuesToFile*
:   True to write values to the file, false to write only to the database

*ppoRetVariables*
:   Array of [IEdmVariableValue6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue6.html) interfaces; one interface for each variable value generated (see **Remarks**)

Generates all default values that have not been generated before.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GenerateDefaultValues( _    ByVal lFolderID As System.Integer, _    ByVal bWriteValuesToFile As System.Boolean, _    ByRef ppoRetVariables() As System.Object _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GenerateDefaultValues(     System.int lFolderID,    System.bool bWriteValuesToFile,    out System.object[] ppoRetVariables ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GenerateDefaultValues(  &   System.int lFolderID, &   System.bool bWriteValuesToFile, &   [Out] System.array<Object^>^ ppoRetVariables ) ``` | |

#### Parameters

*lFolderID*
:   ID of the file's parent folder

*bWriteValuesToFile*
:   True to write values to the file, false to write only to the database

*ppoRetVariables*
:   Array of [IEdmVariableValue6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue6.html) interfaces; one interface for each variable value generated (see **Remarks**)

#### Return Value

True if values were generated, false if not

# ![](dotnetimages/collapse.gif)Remarks

If bWriteValuesToFile is false, then the caller is responsible for writing the values to the file.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: No values needed to be generated.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVariable7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7.html)

[IEdmEnumeratorVariable7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4