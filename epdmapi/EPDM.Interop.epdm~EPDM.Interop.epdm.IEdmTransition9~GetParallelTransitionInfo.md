<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition9~GetParallelTransitionInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetParallelTransitionInfo Method (IEdmTransition9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTransition9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition9.html) : GetParallelTransitionInfo Method (IEdmTransition9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lDocumentID*
:   Document ID

*lProjectID*
:   Project ID

*plReqNum*
:   Number of this parallel transition

*plCommitNum*
:   Number of committed users

*pbRevoke*
:   True to revoke, false to not

Gets the required information for the parallel transition of the specified document and project.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetParallelTransitionInfo( _    ByVal lDocumentID As System.Integer, _    ByVal lProjectID As System.Integer, _    ByRef plReqNum As System.Integer, _    ByRef plCommitNum As System.Integer, _    ByRef pbRevoke As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetParallelTransitionInfo(     System.int lDocumentID,    System.int lProjectID,    out System.int plReqNum,    out System.int plCommitNum,    out System.bool pbRevoke ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetParallelTransitionInfo(  &   System.int lDocumentID, &   System.int lProjectID, &   [Out] System.int plReqNum, &   [Out] System.int plCommitNum, &   [Out] System.bool pbRevoke ) ``` | |

#### Parameters

*lDocumentID*
:   Document ID

*lProjectID*
:   Project ID

*plReqNum*
:   Number of this parallel transition

*plCommitNum*
:   Number of committed users

*pbRevoke*
:   True to revoke, false to not

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTransition9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition9.html)

[IEdmTransition9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition9_members.html)