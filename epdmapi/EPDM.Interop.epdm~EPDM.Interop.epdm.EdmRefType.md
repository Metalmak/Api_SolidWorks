<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmRefType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRefType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of references to return from [IEdmRefItem::GetRefs](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem~GetRefs.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmRefType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmRefType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmRefType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmrt\_Children** | 1 = Return normal file references |
| **Edmrt\_SubParents** | 2 = Return sub-parents, which are parent files displayed as blue children in the reference dialog box; drawing files for some CAD formats are displayed this way |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)