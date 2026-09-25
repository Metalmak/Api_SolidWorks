<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder13~DestroyDeletedItems2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| DestroyDeletedItems2 Method (IEdmFolder13) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder13 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder13.html) : DestroyDeletedItems2 Method (IEdmFolder13) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poDeletedItems*
:   Array of [EdmDeletedItems](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems.html) structures; one structure for each deleted file

*ppoFiles*
:   Array of [EdmFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo.html) structures; one structure for each destroyed file containing information about the file

*poErrors*
:   Array of [EdmBatchDelErrInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo.html) structures; one structure for each destroyed file containing information about errors that occurred during this operation

Destroys the specified deleted items in this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub DestroyDeletedItems2( _    ByVal poDeletedItems() As EdmDeletedItems, _    ByRef ppoFiles() As EdmFileInfo, _    ByRef poErrors() As EdmBatchDelErrInfo _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void DestroyDeletedItems2(     EdmDeletedItems[] poDeletedItems,    out EdmFileInfo[] ppoFiles,    out EdmBatchDelErrInfo[] poErrors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void DestroyDeletedItems2(  &   array<EdmDeletedItems>^ poDeletedItems, &   [Out] array<EdmFileInfo>^ ppoFiles, &   [Out] array<EdmBatchDelErrInfo>^ poErrors ) ``` | |

#### Parameters

*poDeletedItems*
:   Array of [EdmDeletedItems](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems.html) structures; one structure for each deleted file

*ppoFiles*
:   Array of [EdmFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo.html) structures; one structure for each destroyed file containing information about the file

*poErrors*
:   Array of [EdmBatchDelErrInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo.html) structures; one structure for each destroyed file containing information about errors that occurred during this operation

# ![](dotnetimages/collapse.gif)Example

[Destroy Deleted Files in Vault (VB.NET)](Destroy_Deleted_Files_in_Vault_Example_VBNET.htm)

[Destroy Deleted Files in Vault (C#)](Destroy_Deleted_Files_in_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder13 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder13.html)

[IEdmFolder13 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder13_members.html)

[IEdmFolder11::RecoverDeletedItems Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11~RecoverDeletedItems.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2022