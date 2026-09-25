<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsAddDefaultStaticStudyPlotResultError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsAddDefaultStaticStudyPlotResultError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsAddDefaultStaticStudyPlotResultError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Static study result plot errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsAddDefaultStaticStudyPlotResultError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsAddDefaultStaticStudyPlotResultError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsAddDefaultStaticStudyPlotResultError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsAddDefaultStaticStudyPlotResultError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsStaticResultDisplacementComponentRangeError** | 3 = The value of the displacement component is not within the supported range |
| **swsStaticResultElementalStrainRangeError** | 5 = The value of the elemental strain component is not within the supported range |
| **swsStaticResultElementalStressComponentRangeError** | 2 = The value of the elemental stress component is not within the supported range |
| **swsStaticResultNodalStrainRangeError** | 4 = The value of the nodal strain component is not within the supported range |
| **swsStaticResultNodalStressComponentRangeError** | 6 = The value of the nodal stress component is not within the supported range |
| **swsStaticResultNoErrror** | 0 = No error |
| **swsStaticResultTypeRangeError** | 1 = The result type is not supported or is an invalid result type |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)