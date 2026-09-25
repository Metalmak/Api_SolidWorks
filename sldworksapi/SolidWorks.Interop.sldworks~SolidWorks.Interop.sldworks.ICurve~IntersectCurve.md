<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IntersectCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IntersectCurve Method (ICurve) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : IntersectCurve Method (ICurve) |

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
:   Array containing the start point of this curve

*ThisEndPoint*
:   Array containing the end point of this curve

*OtherStartPoint*
:   Array containing the start point of otherCurve

*OtherEndPoint*
:   Array containing the end point of otherCurve

Gets a set of points that represent the intersection of two trimmed curves.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IntersectCurve( _    ByVal OtherCurve As System.Object, _    ByVal ThisStartPoint As System.Object, _    ByVal ThisEndPoint As System.Object, _    ByVal OtherStartPoint As System.Object, _    ByVal OtherEndPoint As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim OtherCurve As System.Object Dim ThisStartPoint As System.Object Dim ThisEndPoint As System.Object Dim OtherStartPoint As System.Object Dim OtherEndPoint As System.Object Dim value As System.Object   value = instance.IntersectCurve(OtherCurve, ThisStartPoint, ThisEndPoint, OtherStartPoint, OtherEndPoint) ``` | |

| C# |  |
| --- | --- |
| ``` System.object IntersectCurve(     System.object OtherCurve,    System.object ThisStartPoint,    System.object ThisEndPoint,    System.object OtherStartPoint,    System.object OtherEndPoint ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ IntersectCurve(  &   System.Object^ OtherCurve, &   System.Object^ ThisStartPoint, &   System.Object^ ThisEndPoint, &   System.Object^ OtherStartPoint, &   System.Object^ OtherEndPoint ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OtherCurve*
:   Curve to intersect with this [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

*ThisStartPoint*
:   Array containing the start point of this curve

*ThisEndPoint*
:   Array containing the end point of this curve

*OtherStartPoint*
:   Array containing the start point of otherCurve

*OtherEndPoint*
:   Array containing the end point of otherCurve

#### Return Value

Array containing the intersection points (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::IntersectCurve.

# ![](dotnetimages/collapse.gif)Remarks

The array of doubles returned contains the x, y, z location of the tessellation points and a code for each point that indicates the intersection class:

[ x1, y1, z1, k1, x2, y2, z2, k2.... ]

Return codes are defined in swIntersectionType\_e.

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::IIntersectCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IIntersectCurve.html)

[ICurve::IIntersectCurveSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IIntersectCurveSize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 98Plus, datecode 1998319