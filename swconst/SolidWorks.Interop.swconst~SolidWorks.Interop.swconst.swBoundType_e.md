<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swBoundType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swBoundType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swBoundType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Boundary behaviors at the start and end of UV parameter ranges.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swBoundType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swBoundType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swBoundType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swBoundType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swBoundType\_Degenerate** | 13741 (**see Remarks**) |
| **swBoundType\_Extendable** | 13734 |
| **swBoundType\_Infinite** | 13733 |
| **swBoundType\_NotExtendable** | 13735 |
| **swBoundType\_Periodic** | 13701 |
| **swBoundType\_PeriodicNotDifferentiable** | 13736 = Not continuously differentiable across the boundary. |

# ![](dotnetimages/collapse.gif)Remarks

If the behavior at the start of the U range is Degenerate', then the V parameter is degenerate when U = urange[0]'. The derivative of the parameterization function with respect to v is 0 whenever u = urange[0]', for all values of v, and the parameter curve corresponding to u = urange[0]' degenerates to a single point. A parameterization can only degenerate at the end of its range, unless the surface is a B-spline surface.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)