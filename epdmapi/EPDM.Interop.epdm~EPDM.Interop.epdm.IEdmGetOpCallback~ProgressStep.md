<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~ProgressStep.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ProgressStep Method (IEdmGetOpCallback) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmGetOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback.html) : ProgressStep Method (IEdmGetOpCallback) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eType*
:   Type of progress bar as defined in [EdmProgressType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmProgressType.html)

*bsMessage*
:   Full path to the processed file

*lProgressPos*
:   New position of the progress bar pointer

Updates the progress bar.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function ProgressStep( _    ByVal eType As EdmProgressType, _    ByVal bsMessage As System.String, _    ByVal lProgressPos As System.Integer _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ProgressStep(     EdmProgressType eType,    System.string bsMessage,    System.int lProgressPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ProgressStep(  &   EdmProgressType eType, &   System.String^ bsMessage, &   System.int lProgressPos ) ``` | |

#### Parameters

*eType*
:   Type of progress bar as defined in [EdmProgressType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmProgressType.html)

*bsMessage*
:   Full path to the processed file

*lProgressPos*
:   New position of the progress bar pointer

#### Return Value

True to continue, false to cancel the operation

# ![](dotnetimages/collapse.gif)Remarks

This method is called periodically by SOLIDWORKS PDM Professional during the operation. [IEdmGetOpCallback::ProgressBegin](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~ProgressBegin.html) is called before this method is called. Implement this method to update a progress bar and to implement a button that, when clicked, halts the operation.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmGetOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback.html)

[IEdmGetOpCallback Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.3