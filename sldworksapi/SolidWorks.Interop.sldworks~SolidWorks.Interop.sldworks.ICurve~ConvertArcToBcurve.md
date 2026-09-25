<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~ConvertArcToBcurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ConvertArcToBcurve Method (ICurve) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : ConvertArcToBcurve Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Center*
:   Array for the x, y, z coordinates of the center point of the
    arc

*Axis*
:   Array for the normal vector of the arc

*Start*
:   Array for the x, y, z coordinates of the start point of the arc

*End*
:   Array for the x, y, z coordinates of the end point of the arc

Gets the b-spline value representation of the arc.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ConvertArcToBcurve( _    ByVal Center As System.Object, _    ByVal Axis As System.Object, _    ByVal Start As System.Object, _    ByVal End As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim Center As System.Object Dim Axis As System.Object Dim Start As System.Object Dim End As System.Object Dim value As System.Object   value = instance.ConvertArcToBcurve(Center, Axis, Start, End) ``` | |

| C# |  |
| --- | --- |
| ``` System.object ConvertArcToBcurve(     System.object Center,    System.object Axis,    System.object Start,    System.object End ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ ConvertArcToBcurve(  &   System.Object^ Center, &   System.Object^ Axis, &   System.Object^ Start, &   System.Object^ End ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Center*
:   Array for the x, y, z coordinates of the center point of the
    arc

*Axis*
:   Array for the normal vector of the arc

*Start*
:   Array for the x, y, z coordinates of the start point of the arc

*End*
:   Array for the x, y, z coordinates of the end point of the arc

#### Return Value

Array for the b-spline representation of the arc

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::ConvertArcToBcurve.

# ![](dotnetimages/collapse.gif)Remarks

Given coordinates of the center, start, end points and the normal vector of an arc, this method returns the b-spline representation of the arc.

The returned data are doubles arranged in the following order:

|  |  |  |
| --- | --- | --- |
| * dim, order | | Two integers packed into a double. |
|  | * dim | Dimension of the control point data.  If dim=3 (non-rational), control point coordinates are returned as [x0,y0,z0,x1,y1,z1,.....].  If dim=4 (rational), control point coordinates are returned as [x0,y0,z0,w0,x1,y1,z1,w1,.....], where w is the weight for the point. |
|  | * order | Order of the b-spline returned. |
| * NumControlPoints, Periodic | | Two integers packed into a double. |
|  | * NumControlPoints | Number of control points for the b-spline. |
|  | * Periodic | True if the b-spline is periodic. |
| * Knots | | Knot vectors. The Knot array contains (NumControlPoints + order) knot values. If the original curve is periodic, then the data is returned in a non-periodic form with extra knots inserted at the curve ends. |
| * ControlPoints | | List of control points output in (NumControlPoints) vectors of dimension dim.  For non-rational b-spline, control point coordinates are output as [x0,y0,z0,x1,y1,z1,.........].  For rational b-spline, control point coordinates and the weight are output as [x0,y0,z0,w0,x1,y1,z1,w1,........], where w is the weight for the point. |

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::ConvertLineToBcurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~ConvertLineToBcurve.html)

[ICurve::GetBCurveParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~GetBCurveParams.html)

[ICurve::IGetBCurveParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IGetBCurveParams.html)

[ICurve::MakeBsplineCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~MakeBsplineCurve.html)