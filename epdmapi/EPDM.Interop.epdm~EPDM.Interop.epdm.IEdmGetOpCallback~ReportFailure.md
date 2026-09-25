<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~ReportFailure.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ReportFailure Method (IEdmGetOpCallback) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmGetOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback.html) : ReportFailure Method (IEdmGetOpCallback) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of affected file

*bsPath*
:   Path to the affected file

*hError*
:   Error code

*bsDetails*
:   Detailed description of the error

Obsolete. Superseded by [IEdmGetOpCallback2::ReportFailureEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback2~ReportFailureEx.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function ReportFailure( _    ByVal lFileID As System.Integer, _    ByVal bsPath As System.String, _    ByVal hError As System.Integer, _    ByVal bsDetails As System.String _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ReportFailure(     System.int lFileID,    System.string bsPath,    System.int hError,    System.string bsDetails ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ReportFailure(  &   System.int lFileID, &   System.String^ bsPath, &   System.int hError, &   System.String^ bsDetails ) ``` | |

#### Parameters

*lFileID*
:   ID of affected file

*bsPath*
:   Path to the affected file

*hError*
:   Error code

*bsDetails*
:   Detailed description of the error

#### Return Value

True to continue, false to cancel the operation

# ![](dotnetimages/collapse.gif)Remarks

SOLIDWORKS PDM Professional calls this method when an error related to a specific file has occurred. Implement this method to display a message box to the user or to automatically process the error.

This method is extended by [IEdmGetOpCallback2::ReportFailureEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback2~ReportFailureEx.html) which provides support for recovering from archive file errors.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmGetOpCallback Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback.html)

[IEdmGetOpCallback Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.3