<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~ProgressBegin.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ProgressBegin Method (IEdmUnlockOpCallback) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUnlockOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html) : ProgressBegin Method (IEdmUnlockOpCallback) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eType*
:   Type of progress bar to start as defined in [EdmProgressType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmProgressType.html)

*eEvent*
:   Type of operation as defined in [EdmUnlockEvent](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockEvent.html)

*lSteps*
:   Number of steps in the operation (see **Remarks**)

Called by the check-in operation when it starts.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub ProgressBegin( _    ByVal eType As EdmProgressType, _    ByVal eEvent As EdmUnlockEvent, _    ByVal lSteps As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void ProgressBegin(     EdmProgressType eType,    EdmUnlockEvent eEvent,    System.int lSteps ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ProgressBegin(  &   EdmProgressType eType, &   EdmUnlockEvent eEvent, &   System.int lSteps ) ``` | |

#### Parameters

*eType*
:   Type of progress bar to start as defined in [EdmProgressType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmProgressType.html)

*eEvent*
:   Type of operation as defined in [EdmUnlockEvent](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockEvent.html)

*lSteps*
:   Number of steps in the operation (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmUnlockOpCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[IEdmUnlockOpCallback::ProgressStep](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~ProgressStep.html) and [IEdmUnlockOpCallback::ProgressStepEvent](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~ProgressStepEvent.html) are each called lStep times. [IEdmUnlockOpCallback::ProgressEnd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~ProgressEnd.html) is called when the operation completes.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUnlockOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html)

[IEdmUnlockOpCallback Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.3