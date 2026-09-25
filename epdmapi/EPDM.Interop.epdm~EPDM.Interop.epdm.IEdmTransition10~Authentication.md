<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition10~Authentication.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Authentication Property (IEdmTransition10) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTransition10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition10.html) : Authentication Property (IEdmTransition10) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets whether this workflow transition requires a password.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property Authentication As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Authentication {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool Authentication {    System.bool get(); } ``` | |

#### Property Value

True if this workflow transition requires a password, false if not

# ![](dotnetimages/collapse.gif)Example

See the [IEdmTransition10](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition10.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This property corresponds to the **Authentication** check box in the Properties dialog of a transition.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTransition10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition10.html)

[IEdmTransition10 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition10_members.html)

[IEdmBatchChangeState4::ChangeState2 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState4~ChangeState2.html)

[IEdmFile10::ChangeState2 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile10~ChangeState2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2015 SP02