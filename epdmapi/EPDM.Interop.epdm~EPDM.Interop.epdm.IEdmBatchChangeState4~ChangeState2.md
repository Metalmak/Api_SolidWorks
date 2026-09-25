<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState4~ChangeState2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ChangeState2 Method (IEdmBatchChangeState4) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchChangeState4 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState4.html) : ChangeState2 Method (IEdmBatchChangeState4) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle that is passed to add-ins that are notified about file state changes in the vault

*bsPasswd*
:   Password of user executing the transition

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to receive progress information about the operation

Changes states or revokes transitions of all the files added to this batch using [IEdmBatchChangeState::AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~AddFile.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub ChangeState2( _    ByVal lParentWnd As System.Integer, _    ByVal bsPasswd As System.String, _    Optional ByVal poCallback As EdmCallback _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void ChangeState2(     System.int lParentWnd,    System.string bsPasswd,    EdmCallback poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ChangeState2(  &   System.int lParentWnd, &   System.String^ bsPasswd, &   EdmCallback^ poCallback ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle that is passed to add-ins that are notified about file state changes in the vault

*bsPasswd*
:   Password of user executing the transition

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to receive progress information about the operation

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchChangeState4](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState4.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

The difference between this method and the now obsolete [IEdmBatchChangeState::ChangeState](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~ChangeState.html) is that this method specifies a user password that allows the file to change state if the transition requires authentication ([IEdmTransition10::Authentication](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition10~Authentication.html)).

Before calling this method, you must call [IEdmBatchChangeState::CreateTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~CreateTree.html) if changing states or [IEdmBatchChangeState2::CreateTreeForRevoke](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2~CreateTreeForRevoke.html) if revoking transitions.

[Return codes](ReturnCodes.htm):

* E\_EDM\_STATECHANGE\_FAILED: The password is invalid.* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchChangeState4 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState4.html)

[IEdmBatchChangeState4 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState4_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2015 SP02