<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~ProgressStepEvent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ProgressStepEvent Method (IEdmUnlockOpCallback) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUnlockOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html) : ProgressStepEvent Method (IEdmUnlockOpCallback) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eType*
:   Type of progress bar to advance as defined in [EdmProgressType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmProgressType.html)

*eText*
:   Type of current operation as defined in [EdmUnlockEventMsg](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockEventMsg.html)

*lProgressPos*
:   New position in the progress bar

Called to advance a progress bar.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function ProgressStepEvent( _    ByVal eType As EdmProgressType, _    ByVal eText As EdmUnlockEventMsg, _    ByVal lProgressPos As System.Integer _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ProgressStepEvent(     EdmProgressType eType,    EdmUnlockEventMsg eText,    System.int lProgressPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ProgressStepEvent(  &   EdmProgressType eType, &   EdmUnlockEventMsg eText, &   System.int lProgressPos ) ``` | |

#### Parameters

*eType*
:   Type of progress bar to advance as defined in [EdmProgressType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmProgressType.html)

*eText*
:   Type of current operation as defined in [EdmUnlockEventMsg](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockEventMsg.html)

*lProgressPos*
:   New position in the progress bar

#### Return Value

True to continue the operation, false to cancel it

# ![](dotnetimages/collapse.gif)Example

See the [IEdmUnlockOpCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method or [IEdmUnlockOpCallback::ProgressStep](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~ProgressStep.html) is called for each step in an operation that begins with [IEdmUnlockOpCallback::ProgressBegin](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~ProgressBegin.html).

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUnlockOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html)

[IEdmUnlockOpCallback Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.3