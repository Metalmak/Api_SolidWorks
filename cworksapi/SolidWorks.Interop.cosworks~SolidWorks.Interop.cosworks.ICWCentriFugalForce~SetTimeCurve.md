<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce~SetTimeCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetTimeCurve Method (ICWCentriFugalForce) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWCentriFugalForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce.html) : SetTimeCurve Method (ICWCentriFugalForce) |

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

Obsolete. Superseded by [ICWCentrifugalForce::SetTimeCurve2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce~SetTimeCurve2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetTimeCurve( _    ByVal VarCurveData As System.Object, _    ByRef ErrorCode As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWCentriFugalForce Dim VarCurveData As System.Object Dim ErrorCode As System.Integer Dim value As System.Integer   value = instance.SetTimeCurve(VarCurveData, ErrorCode) ``` | |

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

True to use actual curve, false to use linear variation

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWCentriFugalForce::SetTimeCurve.

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

[ICWCentriFugalForce::GetTimeCurve Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce~GetTimeCurve.html)

[ICWCentriFugalForce::UseTimeCurve Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCentriFugalForce~UseTimeCurve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0