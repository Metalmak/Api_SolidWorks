<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2~GetRevisionNumberIDFromState.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetRevisionNumberIDFromState Method (IEdmRevisionMgr2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevisionMgr2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2.html) : GetRevisionNumberIDFromState Method (IEdmRevisionMgr2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lStateID*
:   ID of workflow state for which to get a revision number (see **Remarks**)

Gets the ID of the revision number used in the specified workflow state.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetRevisionNumberIDFromState( _    ByVal lStateID As System.Integer _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetRevisionNumberIDFromState(     System.int lStateID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetRevisionNumberIDFromState(  &   System.int lStateID ) ``` | |

#### Parameters

*lStateID*
:   ID of workflow state for which to get a revision number (see **Remarks**)

#### Return Value

Revision number ID; 0 if no revision number is found for the specified workflow state

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, set lStateID using [IEdmState5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html).ID.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_WORKFLOW\_STATE\_ID: The supplied state ID is out of bounds.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevisionMgr2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2.html)

[IEdmRevisionMgr2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007 SP03