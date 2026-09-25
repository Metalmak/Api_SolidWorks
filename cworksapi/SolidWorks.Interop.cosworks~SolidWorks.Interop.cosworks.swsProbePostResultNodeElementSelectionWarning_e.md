<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsProbePostResultNodeElementSelectionWarning_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsProbePostResultNodeElementSelectionWarning\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsProbePostResultNodeElementSelectionWarning\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Results probe selection warnings. Bitmask.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsProbePostResultNodeElementSelectionWarning_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsProbePostResultNodeElementSelectionWarning_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsProbePostResultNodeElementSelectionWarning_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsProbePostResultNodeElementSelectionWarning_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsProbePostResultNodeElemSelectionWarning\_FewElemsLieOnBeamGaps** | 0x1 = Elements lie on beam gaps |
| **swsProbePostResultNodeElemSelectionWarning\_FewNodeElemsLieOnNonRenderedBody** | 0x8 = Nodes or elements are on a non-rendered body |
| **swsProbePostResultNodeElemSelectionWarning\_FewNodeElemsNotOnSectionPlane** | 0x2 = Nodes or elements are not on the section plane |
| **swsProbePostResultNodeElemSelectionWarning\_FewNodeElemsOutOfRange** | 0x4 = Nodes or elements are out of range for the given model |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)