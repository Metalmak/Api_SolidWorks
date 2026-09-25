<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateBsplineSurfaceDLL.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateBsplineSurfaceDLL Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : ICreateBsplineSurfaceDLL Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Properties*
:   Contains 8 longs (see **Remarks**)

*UKnotArray*
:   Array of numUKnots doubles (see Remarks)

*VKnotArray*
:   Array of numVKnots doubles (see Remarks)

*ControlPointCoordArray*
:   Array of numCtrlPtCoord doubles (see Remarks)

Creates a B-spline surface in this body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateBsplineSurfaceDLL( _    ByRef Properties As System.Integer, _    ByRef UKnotArray As System.Double, _    ByRef VKnotArray As System.Double, _    ByRef ControlPointCoordArray As System.Double _ ) As Surface ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim Properties As System.Integer Dim UKnotArray As System.Double Dim VKnotArray As System.Double Dim ControlPointCoordArray As System.Double Dim value As Surface   value = instance.ICreateBsplineSurfaceDLL(Properties, UKnotArray, VKnotArray, ControlPointCoordArray) ``` | |

| C# |  |
| --- | --- |
| ``` Surface ICreateBsplineSurfaceDLL(     ref System.int Properties,    ref System.double UKnotArray,    ref System.double VKnotArray,    ref System.double ControlPointCoordArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Surface^ ICreateBsplineSurfaceDLL(  &   System.int% Properties, &   System.double% UKnotArray, &   System.double% VKnotArray, &   System.double% ControlPointCoordArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Properties*
:   Contains 8 longs (see **Remarks**)

*UKnotArray*
:   Array of numUKnots doubles (see Remarks)

*VKnotArray*
:   Array of numVKnots doubles (see Remarks)

*ControlPointCoordArray*
:   Array of numCtrlPtCoord doubles (see Remarks)

#### Return Value

New B-spline [surface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::ICreateBsplineSurfaceDLL.

# ![](dotnetimages/collapse.gif)Remarks

You can use this method with trimming curve creation routines (for example, [ISurface::AddTrimmingLoop2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~AddTrimmingLoop2.html)) to construct a trimmed surface.

The Properties argument contains the following elements. These are integers packed into a double array in the Dispatch version.

* Uorder, Vorder

  * numV\_CtrlPoints, numU\_CtrlPoints

    * Uperiodicity, Vperiodicity

      * DimensionControlPoints, UNUSED ( set = 0 )

The number of elements in UKnotArray is:

> numUKnots = numU\_CtrlPoints + Uorder

The number of elements in VKnotArray is:

> numVKnots = numV\_CtrlPoints + Vorder

The number of elements in ControlPointCoordArray is :

> numCtrlPtCoord =( NumV\_CtrlPoints \* NumU\_CtrlPoints \* DimensionControlPoints )

**NOTE:** The order of the UV control points are reversed if you used [ISurface::GetBSurfParams3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~GetBSurfParams3.html) or [ISurface::IGetBSurfParams](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~IGetBSurfParams.html) to get the data. You do not need to reverse the UV control points; instead, you can switch the UV knots and related parameters.

For periodics, the first knot must have multiplicity = 1 and all excess multiplicity must be imposed on the last knot. Therefore, a valid periodic knot vector would be { 0, 1, 2, 3, 3, 3 } for a cubic curve. The control point on the seam of the closed curve cannot be replicated at both ends; it should occur only at the beginning.

To convert a clamped periodic curve (numKnots = numCtrlPts + Order, ctrlPts replicated, knot multiplicity = order at each end) to a SOLIDWORKS periodic curve, remove all but one of the knots at the beginning of the vector and remove one at the end. Also, remove the last control point to avoid the point replication.

Any existing object created by this method is destroyed if you call this method again.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0