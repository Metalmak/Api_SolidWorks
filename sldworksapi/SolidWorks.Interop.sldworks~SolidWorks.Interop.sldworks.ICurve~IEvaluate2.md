<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IEvaluate2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IEvaluate2 Method (ICurve) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : IEvaluate2 Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Parameter*
:   Curve parameter

*NumberOfDerivatives*
:   Number of derivatives

Evaluates the curve at the specified parameter of the curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IEvaluate2( _    ByVal Parameter As System.Double, _    ByVal NumberOfDerivatives As System.Integer _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim Parameter As System.Double Dim NumberOfDerivatives As System.Integer Dim value As System.Double   value = instance.IEvaluate2(Parameter, NumberOfDerivatives) ``` | |

| C# |  |
| --- | --- |
| ``` System.double IEvaluate2(     System.double Parameter,    System.int NumberOfDerivatives ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double IEvaluate2(  &   System.double Parameter, &   System.int NumberOfDerivatives ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Parameter*
:   Curve parameter

*NumberOfDerivatives*
:   Number of derivatives

#### Return Value

Array of doubles (see Remarks)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::IEvaluate2.

# ![](dotnetimages/collapse.gif)Remarks

To determine a valid parameter range, use [ICurve::GetEndParams](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~GetEndParams.html) or [IEdge::GetCurveParams2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~GetCurveParams2.html).

The format of the return value is an array of (NumberOfDerivatives + 1) \* 3 doubles:

[evaluated point], [evaluated derivative 1],...[evaluated derivative NumberOfDerivatives]

In pseudo mathematical notation, this could be written as:

    P(t)  P(t)/dt  P(t)/dtdt ..........

 In terms of the number of derivatives that can be returned for a curve type, you could write:

|  |  |
| --- | --- |
| Curve type | Maximum number of derivatives |
| Line/circle/ellipse | 2 |
| Intersection curve | 2 |
| Constant parameter line | Determined by underlying surface |
| SP-curve | 2 |
| B-curve | Any number |

where the curve type is from [ICurve::Identity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~Identity.html).

For a curve of type swCurveTypes\_e::TRIMMED\_TYPE, the number of derivatives is determined by the base curve as obtained from [ICurve::GetBaseCurve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~GetBaseCurve.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::Evaluate2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~Evaluate2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP5, Revision Number 15.5