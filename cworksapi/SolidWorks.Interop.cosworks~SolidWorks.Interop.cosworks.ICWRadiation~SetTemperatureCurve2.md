<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRadiation~SetTemperatureCurve2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetTemperatureCurve2 Method (ICWRadiation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRadiation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRadiation.html) : SetTemperatureCurve2 Method (ICWRadiation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VarCurveData*
:   Array of temperature curve data (see **Remarks**)

*ErrorCode*
:   Temperature curve error as defined in [swsTemperatureCurveError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsTemperatureCurveError_e.html)

Sets the temperature curve data for this radiation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetTemperatureCurve2( _    ByVal VarCurveData As System.Object, _    ByRef ErrorCode As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRadiation Dim VarCurveData As System.Object Dim ErrorCode As System.Integer Dim value As System.Boolean   value = instance.SetTemperatureCurve2(VarCurveData, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetTemperatureCurve2(     System.object VarCurveData,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetTemperatureCurve2(  &   System.Object^ VarCurveData, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*VarCurveData*
:   Array of temperature curve data (see **Remarks**)

*ErrorCode*
:   Temperature curve error as defined in [swsTemperatureCurveError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsTemperatureCurveError_e.html)

#### Return Value

-1 or true to use curve, 0 or false to not

# ![](dotnetimages/collapse.gif)Remarks

Temperature curve data array:

> **[***n, x1, y1, x2, y2, x3, y3,...xn, yn* **]**

where:

* n = number of xi,yi pairs

  * xi = temperature value at the *ith* data point

    * yi = property value associated with temperature xi

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRadiation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRadiation.html)

[ICWRadiation Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRadiation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30