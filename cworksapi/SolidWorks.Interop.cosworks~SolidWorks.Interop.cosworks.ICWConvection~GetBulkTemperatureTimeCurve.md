<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~GetBulkTemperatureTimeCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetBulkTemperatureTimeCurve Method (ICWConvection) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWConvection Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection.html) : GetBulkTemperatureTimeCurve Method (ICWConvection) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the bulk temperature versus time curve data for convection.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBulkTemperatureTimeCurve() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWConvection Dim value As System.Object   value = instance.GetBulkTemperatureTimeCurve() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetBulkTemperatureTimeCurve() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetBulkTemperatureTimeCurve(); ``` | |

#### Return Value

Array of bulk temperature-time curve (see Remarks)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWConvection::GetBulkTemperatureTimeCurve.

# ![](dotnetimages/collapse.gif)Remarks

Bulk temperature-time curve array:

> **[** *n, x1, y1, x2, y2, x3, y3,...xn, yn* **]**

where:

* n  = number of xi,yi pairs

  * xi = time value at the *ith* data point

    * yi = bulk temperature at time xi

# ![](dotnetimages/collapse.gif)See Also

####

[ICWConvection Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection.html)

[ICWConvection Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection_members.html)

[ICWConvection::SetBulkTemperatureTimeCurve Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~SetBulkTemperatureTimeCurve.html)

[ICWConvection::UseBulkTemperatureTimeCurve Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~UseBulkTemperatureTimeCurve.html)

[ICWConvection::BulkAmbientTemperature Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~BulkAmbientTemperature.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0