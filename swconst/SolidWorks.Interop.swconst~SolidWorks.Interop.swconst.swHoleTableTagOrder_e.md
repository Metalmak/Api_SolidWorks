<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swHoleTableTagOrder_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swHoleTableTagOrder\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swHoleTableTagOrder\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Method by which to assign tag numbers to holes of the same size.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swHoleTableTagOrder_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swHoleTableTagOrder_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swHoleTableTagOrder_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swHoleTableTagOrder_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swHoleTableTagOrder\_Radial** | 3 = Number holes in order of increasing radial angle from the table view origin, starting at -180 degrees in a counterclockwise direction |
| **swHoleTableTagOrder\_ReduceToolPath** | 2 = Number holes in next nearest order, starting at the table view origin |
| **swHoleTableTagOrder\_XY** | 1 = Number holes in order of their XLoc and YLoc |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)