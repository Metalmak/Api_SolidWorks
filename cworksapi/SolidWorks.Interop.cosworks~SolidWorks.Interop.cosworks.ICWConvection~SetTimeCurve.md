<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~SetTimeCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetTimeCurve Method (ICWConvection) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWConvection Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection.html) : SetTimeCurve Method (ICWConvection) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VarCurveData*
:   Array of time curve data (see **Remarks**)

*ErrorCode*
:   Error as defined in [swsTimeCurveError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsTimeCurveError_e.html)

Obsolete. Superseded by [ICWConvection::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~SetTimeCurve2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetTimeCurve( _    ByVal VarCurveData As System.Object, _    ByRef ErrorCode As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWConvection Dim VarCurveData As System.Object Dim ErrorCode As System.Integer Dim value As System.Integer   value = instance.SetTimeCurve(VarCurveData, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetTimeCurve(     System.object VarCurveData,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetTimeCurve(  &   System.Object^ VarCurveData, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*VarCurveData*
:   Array of time curve data (see **Remarks**)

*ErrorCode*
:   Error as defined in [swsTimeCurveError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsTimeCurveError_e.html)

#### Return Value

1 to use curve, 0 to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWConvection::SetTimeCurve.

# ![](dotnetimages/collapse.gif)Remarks

Time curve array:

> **[** *n, x1, y1, x2, y2, x3, y3,...xn, yn* **]**

where:

* n  = number of xi,yi pairs

  * xi = time value at the *ith* data point

    * yi = property value associated with time xi

# ![](dotnetimages/collapse.gif)See Also

####

[ICWConvection Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection.html)

[ICWConvection Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection_members.html)

[ICWConvection::GetTimeCurve Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~GetTimeCurve.html)

[ICWConvection::UseTimeCurve Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWConvection~UseTimeCurve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0