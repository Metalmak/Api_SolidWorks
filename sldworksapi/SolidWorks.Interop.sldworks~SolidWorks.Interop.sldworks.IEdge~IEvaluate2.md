<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IEvaluate2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IEvaluate2 Method (IEdge) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEdge Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html) : IEvaluate2 Method (IEdge) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Parameter*
:   Curve parameter U value (see **Remarks**)

*NumberOfDerivatives*
:   Number of derivatives (see **Remarks**)

Evaluates the edge for the specified U parameter.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IEvaluate2( _    ByVal Parameter As System.Double, _    ByVal NumberOfDerivatives As System.Integer _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEdge Dim Parameter As System.Double Dim NumberOfDerivatives As System.Integer Dim value As System.Double   value = instance.IEvaluate2(Parameter, NumberOfDerivatives) ``` | |

| C# |  |
| --- | --- |
| ``` System.double IEvaluate2(     System.double Parameter,    System.int NumberOfDerivatives ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double IEvaluate2(  &   System.double Parameter, &   System.int NumberOfDerivatives ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Parameter*
:   Curve parameter U value (see **Remarks**)

*NumberOfDerivatives*
:   Number of derivatives (see **Remarks**)

#### Return Value

Array of doubles  (see Remarks)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Edge::IEvaluate2.

# ![](dotnetimages/collapse.gif)Remarks

Use [IEdge::IGetCurveParams2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IGetCurveParams2.html) to determine the valid range of U parameter values for Parameter.

The returned array contains ((NumberOfDerivatives + 1) \* 3) + 1 doubles:

[evaluated\_point], [evaluated\_derivative\_1],...[evaluated\_derivative\_NumberOfDerivatives, **[***status\_code***]**

where *status\_code* is a packed double. After unpacking *status\_code* into two longs, the lower long value is 1 for success or 0 for error. See the Example in [IEdge::Evaluate2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~Evaluate2.html).

|  |  |
| --- | --- |
| If curve type [ICurve::Identity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~Identity.html) is... | Then the maximum number of derivatives is... |
| Line/circle/ellipse | 2 |
| Intersection curve | 2 |
| Constant parameter line | Determined by underlying surface |
| SP-curve | 2 |
| B-curve | Any number |

For a curve of type swCurveTypes\_e::TRIMMED\_TYPE, the number of derivatives is determined by the base curve as obtained from [ICurve::GetBaseCurve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~GetBaseCurve.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdge Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html)

[IEdge Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge_members.html)

[IEdge::GetCurveParams2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetCurveParams2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP5, Revision Number 15.5