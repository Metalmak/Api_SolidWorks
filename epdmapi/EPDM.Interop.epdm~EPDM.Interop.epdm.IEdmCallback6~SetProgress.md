<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6~SetProgress.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetProgress Method (IEdmCallback6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html) : SetProgress Method (IEdmCallback6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lBarIndex*
:   0-based index of the progress bar

*lPos*
:   Current position

*bsMsg*
:   Message to be displayed

Sets the current progress bar position.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function SetProgress( _    ByVal lBarIndex As System.Integer, _    ByVal lPos As System.Integer, _    ByVal bsMsg As System.String _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetProgress(     System.int lBarIndex,    System.int lPos,    System.string bsMsg ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetProgress(  &   System.int lBarIndex, &   System.int lPos, &   System.String^ bsMsg ) ``` | |

#### Parameters

*lBarIndex*
:   0-based index of the progress bar

*lPos*
:   Current position

*bsMsg*
:   Message to be displayed

#### Return Value

True to continue, false to cancel

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* <any error code>: The calling method terminated.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html)

[IEdmCallback6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0