<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmCardFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmCardFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Options for file data card behavior used in [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html); use these flags to tell SOLIDWORKS PDM Professional what to do when [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html) returns.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmCardFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmCardFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmCardFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmCF\_CloseDlgCancel** | 2 = Close dialog and do not save changes |
| **EdmCF\_CloseDlgOK** | 1 = Close dialog and save changes |
| **EdmCF\_Nothing** | 0 = Do nothing |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)