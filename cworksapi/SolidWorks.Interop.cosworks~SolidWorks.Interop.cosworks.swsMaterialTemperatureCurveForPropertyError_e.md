<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMaterialTemperatureCurveForPropertyError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsMaterialTemperatureCurveForPropertyError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsMaterialTemperatureCurveForPropertyError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Temperature curve data errors for materials

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsMaterialTemperatureCurveForPropertyError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsMaterialTemperatureCurveForPropertyError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsMaterialTemperatureCurveForPropertyError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsMaterialTemperatureCurveForPropertyError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsMaterialTemperatureCurveForPropertyErrorInvalidArray** | 4 = Invalid array |
| **swsMaterialTemperatureCurveForPropertyErrorNeedDataPoints** | 5 = Curve must have at least two data points |
| **swsMaterialTemperatureCurveForPropertyErrorNotAllowed** | 3 = Temperature curve not allowed for Nitinol material |
| **swsMaterialTemperatureCurveForPropertyErrorNotApplicable** | 2 = Temperature curve is not applicable for this property |
| **swsMaterialTemperatureCurveForPropertyErrorPropertyNotDefined** | 1 = Property not defined for this material model |
| **swsMaterialTemperatureCurveForPropertyErrorSuccessful** | 0 = Successful |
| **swsMaterialTemperatureCurveForPropertyErrorTermperatures** | 6 = Temperature values should be monotonically increasing |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)