<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmClientType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmClientType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmClientType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of SOLIDWORKS PDM Professional client; used in calls to [IEdmVault8::ClientType](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8~ClientType.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmClientType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmClientType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmClientType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmct\_ConisioLight** | 2 = SOLIDWORKS PDM Professional Viewer |
| **Edmct\_ConisioLT** | 4 = LT (Version 5.3 and older) |
| **Edmct\_ConisioProf** | 0 = SOLIDWORKS PDM Professional Editor |
| **Edmct\_ConisioStd** | 1 = SOLIDWORKS PDM Professional Contributor |
| **Edmct\_ConisioWeb** | 3 = SOLIDWORKS PDM Professional Web |
| **Edmct\_None** | -1 = No SOLIDWORKS PDM Professional client is installed |
| **Edmct\_Reserved** | Do not use |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)