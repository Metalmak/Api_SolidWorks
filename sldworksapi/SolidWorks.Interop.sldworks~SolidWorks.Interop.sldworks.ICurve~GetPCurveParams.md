<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~GetPCurveParams.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetPCurveParams Method (ICurve) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : GetPCurveParams Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [ICurve::GetPCurveParams2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~GetPCurveParams2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPCurveParams() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim value As System.Object   value = instance.GetPCurveParams() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetPCurveParams() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetPCurveParams(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of doubles describing the parameters of the curve (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::GetPCurveParams.

# ![](dotnetimages/collapse.gif)Example

#

# ![](dotnetimages/collapse.gif)Remarks

This method returns the curve as a series of segments, each of which has this form:

(w0\*a0 + w1\*a1\*t + w2\*a2\*t\*\*2 + w3\*a3\*t\*\*3)

p(t) = --------------------------------------------

(w0 + w1\*t + w2\*t\*\*2 + w3\*t\*\*3)

Where w is the weight coefficient and a is the polynomial coefficient.

The coefficients returned are vectors of dimensions "dim". For example, if the curve is rational, then dimension = 4, and the coefficients returned for each segment are as follows:

(a0x,a0y,a0z,w0),(a1x,a1y,a1z,w1)...

However, if the curve is returned as non-rational, then dimension = 3, and its coefficients are:

(a0x,a0y,a0z),(a1x,a1y,a1z),...

The size of the return value array is (3 + NumberKnots + NumberSegments x Order x Dimension).

The array is as follows:

[ packedDouble1, packedDouble2, packedDouble3, knot1, knot2,..., CoefficientsSegment1[Dimension], CoefficientsSegment2[Dimension],... ]

where:

packedDouble1: Integer pair containing Reserved and Order

packedDouble2: Integer pair containing NumberSegments and Periodicity

packedDouble3: Integer pair containing NumberKnots and Dimension

knot1

knot2

...

CoefficientsSegment1[Dimension]

CoefficientsSegment2[Dimension]

...

The coefficients for each segment start with the constant term and end with the term of highest degree (for example, ConstantX, ConstantY, ConstantZ, AX, AY, AZ, BX, BY, BZ). The total number of coefficients is:

(NumberSegments) x (Order) x (Dimension).

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::Identity Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~Identity.html)

[ICurve::IGetPCurveParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IGetPCurveParams.html)

[ICurve::IGetPCurveParamsSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IGetPCurveParamsSize.html)