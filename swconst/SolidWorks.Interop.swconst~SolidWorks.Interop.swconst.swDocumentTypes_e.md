<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swDocumentTypes_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swDocumentTypes\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swDocumentTypes\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Document types.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swDocumentTypes_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swDocumentTypes_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swDocumentTypes_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swDocumentTypes_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swDocASSEMBLY** | 2 |
| **swDocDRAWING** | 3 |
| **swDocIMPORTED\_ASSEMBLY** | 7; Multi-CAD |
| **swDocIMPORTED\_PART** | 6; Multi-CAD |
| **swDocLAYOUT** | 5 |
| **swDocNONE** | 0 |
| **swDocPART** | 1 |
| **swDocSDM** | 4 |

# ![](dotnetimages/collapse.gif)Remarks

When opening library feature parts, use swDocPART.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)