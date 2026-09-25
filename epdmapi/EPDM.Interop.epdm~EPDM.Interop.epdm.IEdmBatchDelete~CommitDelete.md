<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~CommitDelete.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CommitDelete Method (IEdmBatchDelete) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchDelete Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete.html) : CommitDelete Method (IEdmBatchDelete) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hParentWnd*
:   Parent window handle that is passed to add-ins that are notified about file or folder deletions from the vault

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to provide delete progress feedback to the user

Deletes the files and folders added to the batch by [IEdmBatchDelete::AddFileByID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~AddFileByID.html), [IEdmBatchDelete::AddFileByPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~AddFileByPath.html), and/or [IEdmBatchDelete::AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~AddFolder.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CommitDelete( _    ByVal hParentWnd As System.Integer, _    Optional ByVal poCallback As EdmCallback _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CommitDelete(     System.int hParentWnd,    EdmCallback poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CommitDelete(  &   System.int hParentWnd, &   EdmCallback^ poCallback ) ``` | |

#### Parameters

*hParentWnd*
:   Parent window handle that is passed to add-ins that are notified about file or folder deletions from the vault

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to provide delete progress feedback to the user

#### Return Value

True if no errors occurred, false if errors occurred

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchDelete](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must call [IEdmBatchDelete::ComputePermissions](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~ComputePermissions.html).

If errors occurred during IEdmBatchDelete::CommitDelete, call [IEdmBatchDelete::ShowCommitErrorsDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~ShowCommitErrorsDlg.html) or [IEdmBatchDelete3::GetCommitErrors](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete3~GetCommitErrors.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_NOT\_INITIALIZED: IEdmBatchDelete::ComputePermissions has not been called.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchDelete Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete.html)

[IEdmBatchDelete Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2008