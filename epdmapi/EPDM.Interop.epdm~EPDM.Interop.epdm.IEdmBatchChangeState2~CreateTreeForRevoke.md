<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2~CreateTreeForRevoke.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateTreeForRevoke Method (IEdmBatchChangeState2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchChangeState2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2.html) : CreateTreeForRevoke Method (IEdmBatchChangeState2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsTransition*
:   Name of the workflow state transition to revoke

Computes the file reference tree and checks that the specified transition revocation can be performed for the files added to this batch using [IEdmBatchChangeState::AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~AddFile.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateTreeForRevoke( _    ByVal bsTransition As System.String _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateTreeForRevoke(     System.string bsTransition ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateTreeForRevoke(  &   System.String^ bsTransition ) ``` | |

#### Parameters

*bsTransition*
:   Name of the workflow state transition to revoke

#### Return Value

True if there are any valid files on which to revoke transitions, false if there are no valid files

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchChangeState2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

To include parent files in the file reference tree, call [IEdmBatchChangeState5::IncludeParentsForRevokeTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState5~IncludeParentsForRevokeTree.html).

After calling this method, call [IEdmBatchChangeState::ShowDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~ShowDlg.html) and/or [IEdmBatchChangeState::ChangeState](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~ChangeState.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchChangeState2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2.html)

[IEdmBatchChangeState2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013