<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFatigueLoadHistoryCurveType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsFatigueLoadHistoryCurveType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsFatigueLoadHistoryCurveType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Types of fatigue load history curves

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsFatigueLoadHistoryCurveType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsFatigueLoadHistoryCurveType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsFatigueLoadHistoryCurveType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsFatigueLoadHistoryCurveType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsFatigueLoadHistoryCurveType\_AmplitudeOnly** | 0 = Define curve by one column of data representing amplitude; do not use this option if your study has multiple fatigue events |
| **swsFatigueLoadHistoryCurveType\_SamplingRateAndAmplitude** | 1 = Define curve by one column of data representing amplitude and specify a value in seconds for the sampling rate; do not use this option if your study has multiple fatigue events |
| **swsFatigueLoadHistoryCurveType\_TimeAndAmplitude** | 2 = Define curve by two columns of data representing pairs of time and amplitude; use this option if your study has multiple fatigue events |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)