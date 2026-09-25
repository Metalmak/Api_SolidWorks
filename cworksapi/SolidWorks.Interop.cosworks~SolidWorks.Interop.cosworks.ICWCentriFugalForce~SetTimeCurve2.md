<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce~SetTimeCurve2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetTimeCurve2 Method (ICWCentriFugalForce) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWCentriFugalForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce.html) : SetTimeCurve2 Method (ICWCentriFugalForce) |

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

Defines a time curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetTimeCurve2( _    ByVal VarCurveData As System.Object, _    ByRef ErrorCode As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWCentriFugalForce Dim VarCurveData As System.Object Dim ErrorCode As System.Integer Dim value As System.Boolean   value = instance.SetTimeCurve2(VarCurveData, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetTimeCurve2(     System.object VarCurveData,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetTimeCurve2(  &   System.Object^ VarCurveData, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*VarCurveData*
:   Array of time curve data (see **Remarks**)

*ErrorCode*
:   Error as defined in [swsTimeCurveError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsTimeCurveError_e.html)

#### Return Value

-1 or true to use actual curve, 0 or false to use linear variation

# ![](dotnetimages/collapse.gif)Remarks

Array of time curve data:

> **[** *n, x1, y1, x2, y2, x3, y3,...xn, yn* ]

where:

* n = number of xi,yi pairs

  * xi = time value at the *ith* data point

    * yi = property value associated with time xi

Time curves are used to specify feature variation with time for transient studies.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWCentriFugalForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce.html)

[ICWCentriFugalForce Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30