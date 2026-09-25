<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IIntersectCurveSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IIntersectCurveSize Method (ICurve) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : IIntersectCurveSize Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OtherCurve*
:   Curve to intersect with this curve

*ThisStartPoint*
:   Start point of this curve

*ThisEndPoint*
:   End point of this curve

*OtherStartPoint*
:   Start point of otherCurve

*OtherEndPoint*
:   End point of otherCurve

Gets the size of the array required by [ICurve::IIntersectCurve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IIntersectCurve.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IIntersectCurveSize( _    ByVal OtherCurve As Curve, _    ByRef ThisStartPoint As System.Double, _    ByRef ThisEndPoint As System.Double, _    ByRef OtherStartPoint As System.Double, _    ByRef OtherEndPoint As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim OtherCurve As Curve Dim ThisStartPoint As System.Double Dim ThisEndPoint As System.Double Dim OtherStartPoint As System.Double Dim OtherEndPoint As System.Double Dim value As System.Integer   value = instance.IIntersectCurveSize(OtherCurve, ThisStartPoint, ThisEndPoint, OtherStartPoint, OtherEndPoint) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IIntersectCurveSize(     Curve OtherCurve,    ref System.double ThisStartPoint,    ref System.double ThisEndPoint,    ref System.double OtherStartPoint,    ref System.double OtherEndPoint ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IIntersectCurveSize(  &   Curve^ OtherCurve, &   System.double% ThisStartPoint, &   System.double% ThisEndPoint, &   System.double% OtherStartPoint, &   System.double% OtherEndPoint ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OtherCurve*
:   Curve to intersect with this curve

*ThisStartPoint*
:   Start point of this curve

*ThisEndPoint*
:   End point of this curve

*OtherStartPoint*
:   Start point of otherCurve

*OtherEndPoint*
:   End point of otherCurve

#### Return Value

Size of the array needed to contain the return values of [ICurve::IIntersectCurve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IIntersectCurve.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::IIntersectCurveSize.

# ![](dotnetimages/collapse.gif)Remarks

To get the actual intersection points, call [ICurve::IIntersectCurve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IIntersectCurve.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::IntersectCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IntersectCurve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 98Plus, datecode 1998319