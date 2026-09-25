<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetOpReply.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmGetOpReply Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGetOpReply Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Options for continuing with a command; returned from [IEdmGetOpCallback2::ReportFailureEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback2~ReportFailureEx.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmGetOpReply     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmGetOpReply : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmGetOpReply : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmGetRep\_CallReportFailure** | 0 = Call [IEdmGetOpCallback::ReportFailure](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetOpCallback~ReportFailure.html) |
| **EdmGetRep\_Cancel** | 1 = Cancel the operation |
| **EdmGetRep\_Process** | 3 = Proceed to process the file |
| **EdmGetRep\_Skip** | 2 = Skip the file but proceed with the operation |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)