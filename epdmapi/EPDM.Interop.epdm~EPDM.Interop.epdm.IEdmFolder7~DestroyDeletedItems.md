<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder7~DestroyDeletedItems.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| DestroyDeletedItems Method (IEdmFolder7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder7.html) : DestroyDeletedItems Method (IEdmFolder7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bRecursive*
:   True to return a list containing all of the sub-items, false to return just the root items

*vDeleteDate*
:   Latest delete date of items to destroy; items deleted after this date are not destroyed

*ppoFiles*
:   Array of [EdmFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo.html) structures; one structure for each destroyed file containing information about the file

*poErrors*
:   Array of [EdmBatchDelErrInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo.html) structures; one structure for each destroyed file containing information about errors that occurred during this operation

Obsolete. Superseded by [IEdmFolder13::DestroyDeletedItems2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder13~DestroyDeletedItems2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub DestroyDeletedItems( _    ByVal bRecursive As System.Boolean, _    ByVal vDeleteDate As System.Object, _    ByRef ppoFiles() As EdmFileInfo, _    ByRef poErrors() As EdmBatchDelErrInfo _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void DestroyDeletedItems(     System.bool bRecursive,    System.object vDeleteDate,    out EdmFileInfo[] ppoFiles,    out EdmBatchDelErrInfo[] poErrors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void DestroyDeletedItems(  &   System.bool bRecursive, &   System.Object^ vDeleteDate, &   [Out] array<EdmFileInfo>^ ppoFiles, &   [Out] array<EdmBatchDelErrInfo>^ poErrors ) ``` | |

#### Parameters

*bRecursive*
:   True to return a list containing all of the sub-items, false to return just the root items

*vDeleteDate*
:   Latest delete date of items to destroy; items deleted after this date are not destroyed

*ppoFiles*
:   Array of [EdmFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo.html) structures; one structure for each destroyed file containing information about the file

*poErrors*
:   Array of [EdmBatchDelErrInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo.html) structures; one structure for each destroyed file containing information about errors that occurred during this operation

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder7.html)

[IEdmFolder7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder7_members.html)

[IEdmFolder11::RecoverDeletedItems Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11~RecoverDeletedItems.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 12.0