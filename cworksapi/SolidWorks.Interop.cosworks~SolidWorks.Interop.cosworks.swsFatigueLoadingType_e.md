<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFatigueLoadingType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsFatigueLoadingType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsFatigueLoadingType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Types of fatigue loading

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsFatigueLoadingType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsFatigueLoadingType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsFatigueLoadingType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsFatigueLoadingType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsFatigueLoadingType\_FullyReversed** | 0 = The fatigue event is based on one reference study; all loads and stress components in the reference study reverse their directions simultaneously for the specified number of cycles in the event |
| **swsFatigueLoadingType\_LoadingRatio** | 2 = The fatigue event is based on one reference study; each load and each stress component in the reference study changes its magnitude proportionally from its maximum value (Smax) to a minimum value defined by R\*Smax, where R is the loading ratio; a negative ratio indicates a reversal of the load direction |
| **swsFatigueLoadingType\_NonProportional** | 3 = The fatigue event is based on one reference study; each load and each stress component in the reference study changes its magnitude non-proportionally from its maximum value (Smax) to a minimum value defined by R\*Smax, where R is the loading ratio; a negative ratio indicates a reversal of the load direction |
| **swsFatigueLoadingType\_ZeroBased** | 1 = The fatigue event is based on one reference study; all loads and stress components in the reference study change their magnitudes proportionally from their maximum values as specified by the reference study to zero |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)