<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~ComputePermissions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ComputePermissions Method (IEdmBatchDelete) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchDelete Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete.html) : ComputePermissions Method (IEdmBatchDelete) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bDestroy*
:   True to permanently delete files and folders, false to move files and folders to the recycle bin

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to provide delete progress feedback to the user

Specifies whether files or folders should be permanently deleted or moved to the recycle bin.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function ComputePermissions( _    ByVal bDestroy As System.Boolean, _    Optional ByVal poCallback As EdmCallback _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ComputePermissions(     System.bool bDestroy,    EdmCallback poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ComputePermissions(  &   System.bool bDestroy, &   EdmCallback^ poCallback ) ``` | |

#### Parameters

*bDestroy*
:   True to permanently delete files and folders, false to move files and folders to the recycle bin

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to provide delete progress feedback to the user

#### Return Value

True if no errors occurred, false otherwise

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchDelete](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must add files and folders to the batch using [IEdmBatchDelete::AddFileByID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~AddFileByID.html), [IEdmBatchDelete::AddFileByPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~AddFileByPath.html), and [IEdmBatchDelete::AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~AddFolder.html).

If errors occurred during IEdmBatchDelete::ComputePermissions, call [IEdmBatchDelete::ShowWarningDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete~ShowWarningDlg.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchDelete Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete.html)

[IEdmBatchDelete Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2008