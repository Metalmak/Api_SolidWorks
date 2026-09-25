<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~ProgressBegin.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ProgressBegin Method (IEdmGetOpCallback) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmGetOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback.html) : ProgressBegin Method (IEdmGetOpCallback) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eType*
:   Type of progress bar as defined in [EdmProgressType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmProgressType.html)

*lSteps*
:   Number of times that [IEdmGetOpCallback::ProgressStep](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~ProgressStep.html) is to be called

Marks the beginning of the process.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub ProgressBegin( _    ByVal eType As EdmProgressType, _    ByVal lSteps As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void ProgressBegin(     EdmProgressType eType,    System.int lSteps ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ProgressBegin(  &   EdmProgressType eType, &   System.int lSteps ) ``` | |

#### Parameters

*eType*
:   Type of progress bar as defined in [EdmProgressType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmProgressType.html)

*lSteps*
:   Number of times that [IEdmGetOpCallback::ProgressStep](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~ProgressStep.html) is to be called

# ![](dotnetimages/collapse.gif)Remarks

Implement this method to display a progress bar. After this method is called, SOLIDWORKS PDM Professional calls IEdmGetOpCallback::ProgressStep lSteps times.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmGetOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback.html)

[IEdmGetOpCallback Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.3