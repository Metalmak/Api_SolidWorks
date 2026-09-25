<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition5~FromState.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| FromState Property (IEdmTransition5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTransition5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition5.html) : FromState Property (IEdmTransition5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets the source state of this transition.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property FromState As IEdmState5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmState5 FromState {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property IEdmState5^ FromState {    IEdmState5^ get(); } ``` | |

#### Property Value

[IEdmState5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html); Null if no source state exists (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

A SOLIDWORKS PDM Professional workflow contains one transition, called AddedToFileVault, without a source state. In SOLIDWORKS PDM Professional 5.2, trying to access the FromState property of the AddedToFileVault transition results in an exception with the error code E\_EDM\_STATE\_NOT\_FOUND. In SOLIDWORKS PDM Professional 5.3 and later, the FromState property can be read without exception from the AddedToFileVault transition.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTransition5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition5.html)

[IEdmTransition5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2