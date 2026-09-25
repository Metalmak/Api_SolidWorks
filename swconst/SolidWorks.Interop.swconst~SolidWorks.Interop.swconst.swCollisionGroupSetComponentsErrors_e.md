<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swCollisionGroupSetComponentsErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swCollisionGroupSetComponentsErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swCollisionGroupSetComponentsErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Errors when setting components in collision groups.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swCollisionGroupSetComponentsErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swCollisionGroupSetComponentsErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swCollisionGroupSetComponentsErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swCollisionGroupSetComponentsErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swCollisionGroupSetComponentsErrors\_ComponentsAddedElsewhere** | 2 = One or more components have already been added to a different collision group |
| **swCollisionGroupSetComponentsErrors\_GroupRemoved** | 3 = The specified collision group is no longer available |
| **swCollisionGroupSetComponentsErrors\_InvalidComponents** | 1 = Components from a different assembly cannot be included in this collision detection |
| **swCollisionGroupSetComponentsErrors\_None** | 0 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)