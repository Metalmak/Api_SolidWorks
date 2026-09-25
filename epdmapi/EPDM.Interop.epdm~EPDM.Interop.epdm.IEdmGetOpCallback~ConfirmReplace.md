<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~ConfirmReplace.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ConfirmReplace Method (IEdmGetOpCallback) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmGetOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback.html) : ConfirmReplace Method (IEdmGetOpCallback) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eReason*
:   Reason for calling this method as defined in [EdmGetConfirmReason](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetConfirmReason.html)

*bsPath*
:   Full path to the local file

Gets whether to replace an existing file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function ConfirmReplace( _    ByVal eReason As EdmGetConfirmReason, _    ByVal bsPath As System.String _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ConfirmReplace(     EdmGetConfirmReason eReason,    System.string bsPath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ConfirmReplace(  &   EdmGetConfirmReason eReason, &   System.String^ bsPath ) ``` | |

#### Parameters

*eReason*
:   Reason for calling this method as defined in [EdmGetConfirmReason](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetConfirmReason.html)

*bsPath*
:   Full path to the local file

#### Return Value

True to replace an existing file, false to leave an existing file

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmGetOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback.html)

[IEdmGetOpCallback Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.3