<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFatigueMeanStressCorrectionType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsFatigueMeanStressCorrectionType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsFatigueMeanStressCorrectionType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Mean stress correction options for calculating alternating stresses

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsFatigueMeanStressCorrectionType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsFatigueMeanStressCorrectionType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsFatigueMeanStressCorrectionType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsFatigueMeanStressCorrectionType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsFatigueMeanStressCorrectionType\_Gerber** | 2 = Use the Gerber mean stress correction equation; suitable for ductile materials |
| **swsFatigueMeanStressCorrectionType\_Goodman** | 1 = Use the Goodman mean stress correction equation; suitable for brittle materials |
| **swsFatigueMeanStressCorrectionType\_None** | 0 = Do not use a mean stress correction |
| **swsFatigueMeanStressCorrectionType\_Soderberg** | 3 = Use the Soderberg mean stress correction equation; this is the most conservative method |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)