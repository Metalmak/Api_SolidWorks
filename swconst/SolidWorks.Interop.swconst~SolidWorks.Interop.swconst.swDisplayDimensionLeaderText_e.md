<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swDisplayDimensionLeaderText_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swDisplayDimensionLeaderText\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swDisplayDimensionLeaderText\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Display dimension leaders and text placement.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swDisplayDimensionLeaderText_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swDisplayDimensionLeaderText_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swDisplayDimensionLeaderText_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swDisplayDimensionLeaderText_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swBrokenLeaderAlignedText** | 3 = Leader is broken and the text is aligned with the leader |
| **swBrokenLeaderHorizontalText** | 2 = Leader is broken and the text is horizontal |
| **swSolidLeaderAlignedText** | 1 = Leader is solid (not broken) and the text is aligned with the leader |
| **swSolidLeaderHorizontalText** | 4 = The leader is solid and the text is horizontal; although this value can be applied to any type of dimension where the dimension text is not between the extension lines, it is currently only implemented by SOLIDWORKS for chamfer dimensions |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)