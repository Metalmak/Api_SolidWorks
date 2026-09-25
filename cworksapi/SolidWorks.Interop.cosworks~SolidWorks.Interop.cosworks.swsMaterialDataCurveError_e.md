<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMaterialDataCurveError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsMaterialDataCurveError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsMaterialDataCurveError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Material curve data errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsMaterialDataCurveError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsMaterialDataCurveError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsMaterialDataCurveError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsMaterialDataCurveError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsMaterialDataCurveErrorCannotBeDefined** | 1 = Material data curve cannot be defined for this material model |
| **swsMaterialDataCurveErrorIndexForMooneyRivlinAndOgeden** | 3 = Index must be 0, 1, or 2 for Mooney-Rivlin and Ogeden material models |
| **swsMaterialDataCurveErrorIndexForViscoElastic** | 4 = Index must be 3 or 4 for the Visco-elastic material model |
| **swsMaterialDataCurveErrorIndexValues** | 2 = Valid index values are 0 to 4 |
| **swsMaterialDataCurveErrorInvalidArray** | 5 = Invalid array |
| **swsMaterialDataCurveErrorNeedDataPoints** | 7 = Curve must have at least two data points   * nIndex = 0; simple tension curve* nIndex = 1; planar tension curve* nIndex = 2; biaxial tension curve* nIndex = 3; shear relaxation curve* nIndex = 4; bulk relaxation curve |
| **swsMaterialDataCurveErrorSuccessful** | 0 = Successful |
| **swsMaterialDataCurveErrorTemperatures** | 6 = Temperature values should be monotonically increasing |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)