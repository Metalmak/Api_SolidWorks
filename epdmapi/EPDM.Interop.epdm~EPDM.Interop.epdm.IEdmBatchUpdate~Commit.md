<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate~Commit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Commit Method (IEdmBatchUpdate) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchUpdate Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate.html) : Commit Method (IEdmBatchUpdate) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoRetErrors*
:   Array of [EdmBatchError](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError.html) structures; one structure for each error that occurred during the save operation

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to get more information during the operation

Obsolete. Superseded by [IEdmBatchUpdate2::CommitUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2~CommitUpdate.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Commit( _    ByRef ppoRetErrors() As EdmBatchError, _    Optional ByVal poCallback As EdmCallback _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Commit(     out EdmBatchError[] ppoRetErrors,    EdmCallback poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Commit(  &   [Out] array<EdmBatchError>^ ppoRetErrors, &   EdmCallback^ poCallback ) ``` | |

#### Parameters

*ppoRetErrors*
:   Array of [EdmBatchError](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError.html) structures; one structure for each error that occurred during the save operation

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to get more information during the operation

# ![](dotnetimages/collapse.gif)Remarks

Non-fatal errors are returned in the ppoRetErrors array. Examine the contents of the returned array to determine whether the operation is successful.

See the [IEdmBatchUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate.html) remarks for information about using this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchUpdate Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate.html)

[IEdmBatchUpdate Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.2