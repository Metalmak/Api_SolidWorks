<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsThermalComponent_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsThermalComponent\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsThermalComponent\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Thermal components

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsThermalComponent_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsThermalComponent_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsThermalComponent_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsThermalComponent_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsThermalComponentGRADN** | 4 = Resultant temperature gradient |
| **swsThermalComponentGRADX** | 1 = Temperature gradient in the X direction of the selected reference geometry |
| **swsThermalComponentGRADY** | 2 = Temperature gradient in the Y direction of the selected reference geometry |
| **swsThermalComponentGRADZ** | 3 = Temperature gradient in the Z direction of the selected reference geometry |
| **swsThermalComponentHFLUXN** | 8 = Resultant heat flux |
| **swsThermalComponentHFLUXX** | 5 = Heat flux in the X direction of the selected reference geometry |
| **swsThermalComponentHFLUXY** | 6 = Heat flux in the Y direction of the selected reference geometry |
| **swsThermalComponentHFLUXZ** | 7 = Heat flux in the Z direction of the selected reference geometry |
| **swsThermalComponentTEMP** | 0 = Nodal temperature |

# ![](dotnetimages/collapse.gif)Remarks

X, Y, Z directions correspond to the reference geometry. The first plane that appears in the FeatureManager tree is used as the default reference geometry.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)