<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swFeatureFilletProfileType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swFeatureFilletProfileType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swFeatureFilletProfileType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Fillet cross-sectional profile shapes.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swFeatureFilletProfileType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swFeatureFilletProfileType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swFeatureFilletProfileType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swFeatureFilletProfileType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swFeatureFilletCircular** | 0 = Circular for symmetric fillets; elliptical for asymmetric fillets |
| **swFeatureFilletConicRadius** | 2 = Requires that you set the radius of curvature at the shoulder point along the fillet's cross section |
| **swFeatureFilletConicRho** | 1 = Requires that you set a ratio in the range [0.5, 0.95] which indicates the weight of the cross-section |
| **swFeatureFilletConicRhoZeroChamfer** | 3 = Chamfer cross section |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)