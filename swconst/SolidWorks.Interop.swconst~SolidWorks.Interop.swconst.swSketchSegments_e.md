<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSketchSegments_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swSketchSegments\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swSketchSegments\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Types of ISketchSegment objects.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swSketchSegments_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swSketchSegments_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swSketchSegments_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swSketchSegments_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSketchARC** | 1 |
| **swSketchELLIPSE** | 2 |
| **swSketchLINE** | 0 |
| **swSketchPARABOLA** | 5 |
| **swSketchSPLINE** | 3 |
| **swSketchTEXT** | 4 |

# ![](dotnetimages/collapse.gif)Remarks

Based on these types, you can obtain the appropriate derived class (that is, ISketchLine, ISketchArc, and so on) and call the appropriate derived class functions.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)