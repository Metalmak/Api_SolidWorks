<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swFilletOverFlowType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swFilletOverFlowType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swFilletOverFlowType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Fillet overflow types.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swFilletOverFlowType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swFilletOverFlowType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swFilletOverFlowType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swFilletOverFlowType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swFilletOverFlowType\_Default** | 0 = Default; system picks the appropriate method to create a fillet when the fillet surface overflows to adjacent surfaces; it either smoothly blends with adjacent surfaces or limits the fillet surface with the adjacent edges, thereby not changing the edge, or trims the fillet surface by the adjacent surface onto which the fillet overflows; the method actually used by default depending on the geometric condition; this option always tries to create a fillet if possible |
| **swFilletOverFlowType\_KeepEdge** | 1 = Edges that are overflowed by the fillet are not modified; the fillet surface is trimmed by all the adjacent edges; as a result, an additional transition fillet surface might be needed to complete the fillet |
| **swFilletOverFlowType\_KeepSurface** | 2 = Fillet surface is either merged with the adjacent surfaces smoothly or trimmed by the adjacent surfaces; as a result, it is unlikely that an additional transition fillet surface is created |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)