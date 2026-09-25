<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~ChangeState.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ChangeState Method (IEdmBatchChangeState) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchChangeState Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState.html) : ChangeState Method (IEdmBatchChangeState) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle that is passed to add-ins that are notified about file state changes in the vault

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to receive progress information about the operation

Obsolete. Superseded by [IEdmBatchChangeState4::ChangeState2.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState4~ChangeState2.html)

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub ChangeState( _    ByVal lParentWnd As System.Integer, _    Optional ByVal poCallback As EdmCallback _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void ChangeState(     System.int lParentWnd,    EdmCallback poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ChangeState(  &   System.int lParentWnd, &   EdmCallback^ poCallback ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle that is passed to add-ins that are notified about file state changes in the vault

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to receive progress information about the operation

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must call [IEdmBatchChangeState::CreateTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~CreateTree.html) if changing states or [IEdmBatchChangeState2::CreateTreeForRevoke](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2~CreateTreeForRevoke.html) if revoking transitions.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchChangeState Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState.html)

[IEdmBatchChangeState Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009; for revoking a transition, SOLIDWORKS PDM Professional 2013