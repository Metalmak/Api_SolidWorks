<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~LogMessage.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| LogMessage Method (IEdmGetOpCallback) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmGetOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback.html) : LogMessage Method (IEdmGetOpCallback) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eMsgID*
:   Message to display to the user as defined in [EdmGetOpMsg](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetOpMsg.html)

*hCode*
:   Error code causing this method to be called

*bsDetails*
:   Reason for calling this method

Notifies about an error that occurred during the process.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub LogMessage( _    ByVal eMsgID As EdmGetOpMsg, _    ByVal hCode As System.Integer, _    ByVal bsDetails As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void LogMessage(     EdmGetOpMsg eMsgID,    System.int hCode,    System.string bsDetails ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void LogMessage(  &   EdmGetOpMsg eMsgID, &   System.int hCode, &   System.String^ bsDetails ) ``` | |

#### Parameters

*eMsgID*
:   Message to display to the user as defined in [EdmGetOpMsg](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetOpMsg.html)

*hCode*
:   Error code causing this method to be called

*bsDetails*
:   Reason for calling this method

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmGetOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback.html)

[IEdmGetOpCallback Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.3