<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~ConvertLineToBcurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ConvertLineToBcurve Method (ICurve) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : ConvertLineToBcurve Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StartPoint*
:   Array values for the coordinates of the start point of the line

*EndPoint*
:   Array values for the coordinates of the end point of the line

Converts the specified line into a b-spline curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ConvertLineToBcurve( _    ByVal StartPoint As System.Object, _    ByVal EndPoint As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim StartPoint As System.Object Dim EndPoint As System.Object Dim value As System.Object   value = instance.ConvertLineToBcurve(StartPoint, EndPoint) ``` | |

| C# |  |
| --- | --- |
| ``` System.object ConvertLineToBcurve(     System.object StartPoint,    System.object EndPoint ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ ConvertLineToBcurve(  &   System.Object^ StartPoint, &   System.Object^ EndPoint ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StartPoint*
:   Array values for the coordinates of the start point of the line

*EndPoint*
:   Array values for the coordinates of the end point of the line

#### Return Value

Array values giving the b-spline representation of the line

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::ConvertLineToBcurve.

# ![](dotnetimages/collapse.gif)Remarks

Given coordinates of two end points of a line, this method returns the b-spline representation of the line. The returned data are doubles arranged in the following order:

|  |  |  |
| --- | --- | --- |
| * dim, order | | Two integers packed into a double. |
|  | * dim | Dimension of the control point data.  If dim=3 (non-rational), control point coordinates are returned as [x0,y0,z0,x1,y1,z1,.....].  If dim=4 (rational), control point coordinates are returned as [x0,y0,z0,w0,x1,y1,z1,w1,.....], where w is the weight for the point. |
|  | * order | Order of the b-spline returned. |
| * NumControlPoints, Periodic | | Two integers packed into a double. |
|  | * NumControlPoints | Number of control points for the b-spline. |
|  | * Periodic | True if the b-spline is periodic. |
| * Knots | | Knot vectors. The Knot array contains (NumControlPoints + order) knot values. If the original curve is periodic, then the data is  returned in a non-periodic form with extra knots inserted at the curve ends. |
| * ControlPoints | | List of control points output in (NumControlPoints) vectors of dimension dim.  For non-rational b-spline, control point coordinates are output as [x0,y0,z0,x1,y1,z1,.........].  For rational b-spline, control point coordinates and the weight are output as [x0,y0,z0,w0,x1,y1,z1,w1,........], where w is the weight for the point. |

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::ConvertArcToBcurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~ConvertArcToBcurve.html)

[ICurve::GetBCurveParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~GetBCurveParams.html)

[ICurve::IGetBCurveParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IGetBCurveParams.html)

[ICurve::IsLine Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IsLine.html)

[ICurve::MakeBsplineCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~MakeBsplineCurve.html)