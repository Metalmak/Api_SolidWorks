<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback~SetStatusMessage.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetStatusMessage Method (IEdmCallback) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) : SetStatusMessage Method (IEdmCallback) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsMessage*
:   Message to display

Displays a message to the user.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetStatusMessage( _    ByVal bsMessage As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetStatusMessage(     System.string bsMessage ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetStatusMessage(  &   System.String^ bsMessage ) ``` | |

#### Parameters

*bsMessage*
:   Message to display

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_CANCELLED\_BY\_USER: Cancel the operation.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html)

[IEdmCallback Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2