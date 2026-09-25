<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IIntersectCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IIntersectCurve Method (ICurve) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : IIntersectCurve Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OtherCurve*
:   Curve to intersect with this [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

*ThisStartPoint*
:   Start point of this curve

*ThisEndPoint*
:   End point of this curve

*OtherStartPoint*
:   Start point of otherCurve

*OtherEndPoint*
:   End point of otherCurve

Gets a set of points that represent the intersection of two trimmed curves.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IIntersectCurve( _    ByVal OtherCurve As Curve, _    ByRef ThisStartPoint As System.Double, _    ByRef ThisEndPoint As System.Double, _    ByRef OtherStartPoint As System.Double, _    ByRef OtherEndPoint As System.Double _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim OtherCurve As Curve Dim ThisStartPoint As System.Double Dim ThisEndPoint As System.Double Dim OtherStartPoint As System.Double Dim OtherEndPoint As System.Double Dim value As System.Double   value = instance.IIntersectCurve(OtherCurve, ThisStartPoint, ThisEndPoint, OtherStartPoint, OtherEndPoint) ``` | |

| C# |  |
| --- | --- |
| ``` System.double IIntersectCurve(     Curve OtherCurve,    ref System.double ThisStartPoint,    ref System.double ThisEndPoint,    ref System.double OtherStartPoint,    ref System.double OtherEndPoint ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double IIntersectCurve(  &   Curve^ OtherCurve, &   System.double% ThisStartPoint, &   System.double% ThisEndPoint, &   System.double% OtherStartPoint, &   System.double% OtherEndPoint ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OtherCurve*
:   Curve to intersect with this [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

*ThisStartPoint*
:   Start point of this curve

*ThisEndPoint*
:   End point of this curve

*OtherStartPoint*
:   Start point of otherCurve

*OtherEndPoint*
:   End point of otherCurve

#### Return Value

* in-process, unmanaged C++: Pointer to an array of doubles of the intersection points (see **Remarks**)

* VBA, VB.NET, C#, and C++/CLI: Not supported

See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::IIntersectCurve.

# ![](dotnetimages/collapse.gif)Remarks

The array of doubles returned contains the x, y, z location of the tessellation points and a code for each point that indicates the intersection class:

[ x1, y1, z1, k1, x2, y2, z2, k2.... ]

Return codes are defined in swIntersectionType\_e.

Before calling this method, call [ICurve::IIntersectCurveSize](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IIntersectCurveSize.html) to determine the size of the array needed for the return values from this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::IntersectCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IntersectCurve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 98Plus, datecode 1988319