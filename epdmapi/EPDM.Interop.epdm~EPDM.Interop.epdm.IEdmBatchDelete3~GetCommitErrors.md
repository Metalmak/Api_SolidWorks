<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete3~GetCommitErrors.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetCommitErrors Method (IEdmBatchDelete3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchDelete3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete3.html) : GetCommitErrors Method (IEdmBatchDelete3) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoDelErrors*
:   Array of [EdmBatchDelErrInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo.html) structures; one for each error that occurred during IEdmBatchDelete::CommitDelete

Shows the errors that occurred during [IEdmBatchDelete::CommitDelete](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~CommitDelete.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetCommitErrors( _    ByRef ppoDelErrors() As EdmBatchDelErrInfo _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetCommitErrors(     out EdmBatchDelErrInfo[] ppoDelErrors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetCommitErrors(  &   [Out] array<EdmBatchDelErrInfo>^ ppoDelErrors ) ``` | |

#### Parameters

*ppoDelErrors*
:   Array of [EdmBatchDelErrInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchDelErrInfo.html) structures; one for each error that occurred during IEdmBatchDelete::CommitDelete

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchDelete](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Call this method after calling IEdmBatchDelete::CommitDelete.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_NOT\_INITIALIZED: IEdmBatchDelete::CommitDelete has not been called.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchDelete3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete3.html)

[IEdmBatchDelete3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete3_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2012