<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~ChangeState.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ChangeState Method (IEdmFile5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) : ChangeState Method (IEdmFile5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poStateIdOrName*
:   Workflow state ID or name or [IEdmState5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html) to which this file transitions (see **Remarks**)

*lFolderID*
:   ID of the file's active parent folder

*bsComment*
:   Comment saved to the transition history

*lParentWnd*
:   Parent window handle

*lEdmStateFlags*
:   Optional combination of [EdmStateFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmStateFlags.html) bits; default is EdmStateFlags.EdmState\_Simple

Obsolete. Superseded by [IEdmFile10::ChangeState2.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile10~ChangeState2.html)

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub ChangeState( _    ByRef poStateIdOrName As System.Object, _    ByVal lFolderID As System.Integer, _    ByVal bsComment As System.String, _    ByVal lParentWnd As System.Integer, _    Optional ByVal lEdmStateFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void ChangeState(     ref System.object poStateIdOrName,    System.int lFolderID,    System.string bsComment,    System.int lParentWnd,    System.int lEdmStateFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ChangeState(  &   System.Object^% poStateIdOrName, &   System.int lFolderID, &   System.String^ bsComment, &   System.int lParentWnd, &   System.int lEdmStateFlags ) ``` | |

#### Parameters

*poStateIdOrName*
:   Workflow state ID or name or [IEdmState5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html) to which this file transitions (see **Remarks**)

*lFolderID*
:   ID of the file's active parent folder

*bsComment*
:   Comment saved to the transition history

*lParentWnd*
:   Parent window handle

*lEdmStateFlags*
:   Optional combination of [EdmStateFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmStateFlags.html) bits; default is EdmStateFlags.EdmState\_Simple

# ![](dotnetimages/collapse.gif)Remarks

There must be a transition between the current state and poStateIdOrName, or this method fails.

It is possible to create multiple workflows with two or more states having the same name. If poStateIdOrName contains the name of the destination state instead of its ID, and if several transitions from the file’s current state lead to new states all having the same name, SOLIDWORKS PDM Professional randomly selects one of them. To be sure to which state the file transitions, specify a state ID in poStateIdOrName.

See [Return Codes](ReturnCodes.htm) for the complete list of potential success and error codes. The following are just a few examples:

* S\_OK: The method successfully executed.* E\_EDM\_TRANSITION\_ACTION\_FAILED: One of the transition actions set up in the workflow failed.* E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN: One of the [EdmCmdType.EdmCmd\_PreState](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html) hooks did not permit the operation.* E\_EDM\_FILE\_IS\_LOCKED: The file is checked out. Changing state is only permitted on checked-in files.* E\_EDM\_PERMISSION\_DENIED: The logged-in user lacks permission to change state.* E\_EDM\_CONDITIONS\_NOT\_MET: The conditions set up in the Workflow Editor for this transition were not met.* E\_EDM\_STATE\_NOT\_FOUND: There is no transition going from the file's current state to the specified state.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[IEdmFile5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html)

[IEdmWorkflow5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow5.html)

[IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html)

[IEdmTransition5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition5.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2