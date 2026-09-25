<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback8~SetMinorProgress.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetMinorProgress Method (IEdmCallback8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCallback8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback8.html) : SetMinorProgress Method (IEdmCallback8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oMsg*
:   Message to be displayed

*dwProgress*
:   Progress

Sets the current minor progress bar position.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetMinorProgress( _    ByVal oMsg As System.String, _    ByVal dwProgress As System.UInteger _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMinorProgress(     System.string oMsg,    System.uint dwProgress ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMinorProgress(  &   System.String^ oMsg, &   System.uint dwProgress ) ``` | |

#### Parameters

*oMsg*
:   Message to be displayed

*dwProgress*
:   Progress

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCallback8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback8.html)

[IEdmCallback8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2021