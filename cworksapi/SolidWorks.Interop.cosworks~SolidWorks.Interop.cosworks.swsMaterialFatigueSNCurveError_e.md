<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMaterialFatigueSNCurveError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsMaterialFatigueSNCurveError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsMaterialFatigueSNCurveError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Material stress-number (SN) curve data errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsMaterialFatigueSNCurveError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsMaterialFatigueSNCurveError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsMaterialFatigueSNCurveError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsMaterialFatigueSNCurveError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsMaterialFatigueSNCurveErrorCurveDataPoints** | 4 = Curve must have at least two data points |
| **swsMaterialFatigueSNCurveErrorCycles** | 3 = Cycle values should be monotonically increasing |
| **swsMaterialFatigueSNCurveErrorIndexValues** | 1 = Valid index values are 0 to 9 |
| **swsMaterialFatigueSNCurveErrorInvalidArray** | 2 = Invalid array |
| **swsMaterialFatigueSNCurveErrorStressValuesMustBeUnique** | 5 = Stress values must be unique for each number of cycles |
| **swsMaterialFatigueSNCurveErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)