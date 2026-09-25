<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback~SetProgressRange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetProgressRange Method (IEdmCallback) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) : SetProgressRange Method (IEdmCallback) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lMin*
:   Minimum value in the progress bar

*lMax*
:   Maximum value in the progress bar

Sets the minimum and maximum values in the progress bar.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetProgressRange( _    ByVal lMin As System.Integer, _    ByVal lMax As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetProgressRange(     System.int lMin,    System.int lMax ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetProgressRange(  &   System.int lMin, &   System.int lMax ) ``` | |

#### Parameters

*lMin*
:   Minimum value in the progress bar

*lMax*
:   Maximum value in the progress bar

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_CANCELLED\_BY\_USER: Cancel the operation.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html)

[IEdmCallback Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback_members.html)

[IEdmCallback::SetProgressPos Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback~SetProgressPos.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2