<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetTimeOrFrequencyCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetTimeOrFrequencyCurve Method (ICWBaseExcitation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html) : SetTimeOrFrequencyCurve Method (ICWBaseExcitation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VarCurveData*
:   Array (see Remarks)

*ErrorCode*
:   0 if successful, 1 if not

Obsolete. Superseded by [ICWBaseExcitation::SetTimeOrFrequencyCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetTimeOrFrequencyCurve2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetTimeOrFrequencyCurve( _    ByVal VarCurveData As System.Object, _    ByRef ErrorCode As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBaseExcitation Dim VarCurveData As System.Object Dim ErrorCode As System.Integer Dim value As System.Integer   value = instance.SetTimeOrFrequencyCurve(VarCurveData, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetTimeOrFrequencyCurve(     System.object VarCurveData,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetTimeOrFrequencyCurve(  &   System.Object^ VarCurveData, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*VarCurveData*
:   Array (see Remarks)

*ErrorCode*
:   0 if successful, 1 if not

#### Return Value

1 to use the time or frequency curve, 0 to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWBaseExcitation::SetTimeOrFrequencyCurve.

# ![](dotnetimages/collapse.gif)Remarks

Array of linear or curve data:

> **[** *n, x1, y1, x2, y2, x3, y3,...xn, yn* **]**

where for modal time history and nonlinear dynamic studies:

* n = number of xi,yi pairs

  * xi = time value at the *ith* data point

    * yi = excitation value associated with time xi

and for harmonic and random vibration dynamic studies:

* n = number of xi,yi pairs

  * xi = frequency value at the *ith* data point

    * yi = excitation value associated with frequency xi

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html)

[ICWBaseExcitation Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation_members.html)

[ICWBaseExcitation::GetTimeOrFrequencyCurve Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetTimeOrFrequencyCurve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0