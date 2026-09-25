<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2~CommitUpdate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CommitUpdate Method (IEdmBatchUpdate2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchUpdate2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2.html) : CommitUpdate Method (IEdmBatchUpdate2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoRetErrors*
:   Array of [EdmBatchError2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError2.html) structures; one structure for each non-critical error that occurred during the update

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to get more information during the operation

Commits all of the file and folder card variable updates in this batch.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CommitUpdate( _    ByRef ppoRetErrors() As EdmBatchError2, _    Optional ByVal poCallback As EdmCallback _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int CommitUpdate(     out EdmBatchError2[] ppoRetErrors,    EdmCallback poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CommitUpdate(  &   [Out] array<EdmBatchError2>^ ppoRetErrors, &   EdmCallback^ poCallback ) ``` | |

#### Parameters

*ppoRetErrors*
:   Array of [EdmBatchError2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchError2.html) structures; one structure for each non-critical error that occurred during the update

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to get more information during the operation

#### Return Value

Size of ppoRetErrors array; 0 if no errors

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchUpdate2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchUpdate2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2.html)

[IEdmBatchUpdate2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.3