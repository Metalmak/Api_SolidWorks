<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRandomVibrationCorrelationOption_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsRandomVibrationCorrelationOption\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsRandomVibrationCorrelationOption\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Options for load correlation in random vibration dynamic studies

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsRandomVibrationCorrelationOption_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsRandomVibrationCorrelationOption_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsRandomVibrationCorrelationOption_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsRandomVibrationCorrelationOption_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsRandomVibrationCorrelationOption\_FullyCorrelated** | 0 = Fully correlated; the distance between load nodes is smaller than a user-defined minimum radius |
| **swsRandomVibrationCorrelationOption\_FullyUnCorrelated** | 1 = Fully uncorrelated; the distance between load nodes is larger than a user-defined maximum radius |
| **swsRandomVibrationCorrelationOption\_PartiallyCorrelated** | 2 = Partially correlated; the distance between load nodes is between a user-defined minimum radius and a user-defined maximum radius |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)