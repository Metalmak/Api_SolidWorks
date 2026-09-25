<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~AddTrimmingLoop2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddTrimmingLoop2 Method (ISurface) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : AddTrimmingLoop2 Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NCrvs*
:   Number of surface parametric (UV) curves constituting the loop and the size of each of the VOrder, VDim, VPeriodic, VNumKnots, VNumControlPnts arrays

*VOrder*
:   Array containing NCrvs longs (VBA), Integers (VB.NET), or ints (C#, C++) representing orders of the curves (see **Remarks**)

*VDim*
:   Array containing NCrvs longs (VBA), Integers (VB.NET), or ints (C#, C++) representing dimensions (2, 3, or 4) of the control points of the curves (see **Remarks**)

*VPeriodic*
:   Array containing NCrvs longs (VBA), Integers (VB.NET), or ints (C#, C++) representing whether the curve is periodic (1) or non-periodic (0) (see **Remarks**)

*VNumKnots*
:   Array containing NCrvs longs (VBA), Integers (VB.NET), or ints (C#, C++) representing number of knots on the curves (see **Remarks**)

*VNumCtrlPoints*
:   Array containing NCrvs longs (VBA), Integers (VB.NET), or ints (C#, C++) representing number of control points on the curves (see **Remarks**)

*VKnots*
:   Knot vector array of <TotalNumKnots> doubles, where TotalNumKnots = (TotalNumKnots + VNumKnots[i]) for i = 1 to NCrvs (see **Remarks**)

*VCtrlPointDbls*
:   Control point coordinate array of <TotalNumCPCoords> doubles, where TotalNumCPCoords = (TotalNumCPCoords + (VDim[i] \* VNumCtrlPoints[i])) for i = 1 to NCrvs (see **Remarks**)

*UvRange*
:   Array of four doubles representing U Low, U High, V Low, and V High (see **Remarks**)

Creates a trimming loop out of specified surface parametric UV-curves and adds it to a list of such loops.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddTrimmingLoop2( _    ByVal NCrvs As System.Integer, _    ByVal VOrder As System.Object, _    ByVal VDim As System.Object, _    ByVal VPeriodic As System.Object, _    ByVal VNumKnots As System.Object, _    ByVal VNumCtrlPoints As System.Object, _    ByVal VKnots As System.Object, _    ByVal VCtrlPointDbls As System.Object, _    ByVal UvRange As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim NCrvs As System.Integer Dim VOrder As System.Object Dim VDim As System.Object Dim VPeriodic As System.Object Dim VNumKnots As System.Object Dim VNumCtrlPoints As System.Object Dim VKnots As System.Object Dim VCtrlPointDbls As System.Object Dim UvRange As System.Object Dim value As System.Boolean   value = instance.AddTrimmingLoop2(NCrvs, VOrder, VDim, VPeriodic, VNumKnots, VNumCtrlPoints, VKnots, VCtrlPointDbls, UvRange) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddTrimmingLoop2(     System.int NCrvs,    System.object VOrder,    System.object VDim,    System.object VPeriodic,    System.object VNumKnots,    System.object VNumCtrlPoints,    System.object VKnots,    System.object VCtrlPointDbls,    System.object UvRange ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddTrimmingLoop2(  &   System.int NCrvs, &   System.Object^ VOrder, &   System.Object^ VDim, &   System.Object^ VPeriodic, &   System.Object^ VNumKnots, &   System.Object^ VNumCtrlPoints, &   System.Object^ VKnots, &   System.Object^ VCtrlPointDbls, &   System.Object^ UvRange ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NCrvs*
:   Number of surface parametric (UV) curves constituting the loop and the size of each of the VOrder, VDim, VPeriodic, VNumKnots, VNumControlPnts arrays

*VOrder*
:   Array containing NCrvs longs (VBA), Integers (VB.NET), or ints (C#, C++) representing orders of the curves (see **Remarks**)

*VDim*
:   Array containing NCrvs longs (VBA), Integers (VB.NET), or ints (C#, C++) representing dimensions (2, 3, or 4) of the control points of the curves (see **Remarks**)

*VPeriodic*
:   Array containing NCrvs longs (VBA), Integers (VB.NET), or ints (C#, C++) representing whether the curve is periodic (1) or non-periodic (0) (see **Remarks**)

*VNumKnots*
:   Array containing NCrvs longs (VBA), Integers (VB.NET), or ints (C#, C++) representing number of knots on the curves (see **Remarks**)

*VNumCtrlPoints*
:   Array containing NCrvs longs (VBA), Integers (VB.NET), or ints (C#, C++) representing number of control points on the curves (see **Remarks**)

*VKnots*
:   Knot vector array of <TotalNumKnots> doubles, where TotalNumKnots = (TotalNumKnots + VNumKnots[i]) for i = 1 to NCrvs (see **Remarks**)

*VCtrlPointDbls*
:   Control point coordinate array of <TotalNumCPCoords> doubles, where TotalNumCPCoords = (TotalNumCPCoords + (VDim[i] \* VNumCtrlPoints[i])) for i = 1 to NCrvs (see **Remarks**)

*UvRange*
:   Array of four doubles representing U Low, U High, V Low, and V High (see **Remarks**)

#### Return Value

True if successful in adding a trimming loop to the surface, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::AddTrimmingLoop2.

# ![](dotnetimages/collapse.gif)Example

[Create Body Using Trimmed Surfaces (VBA)](Create_Body_using_Trimmed_Surfaces_Example_VB.htm)

[Create Body Using Trimmed Surfaces (VB.NET)](Create_Body_using_Trimmed_Surfaces_Example_VBNET.htm)

[Create Body Using Trimmed Surfaces (C#)](Create_Body_using_Trimmed_Surfaces_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The list of trimming loops is created by a previous call to one of the base surface creation functions, [IBody2::CreateRevolutionSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateRevolutionSurface.html) or [IBody2::CreatePlanarSurface.](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreatePlanarSurface.html)

The information on each UV-curve is in b-spline form (knots and control point coordinates) and is compacted into two arrays, VKnots and VCtrlPointDbls.

Order of each curve in VOrder is, at a minimum, 2. A second order curve is a linear curve.

For each curve in VNumCtrlPoints, VOrder, and VNumKnots, (NumCtrlPoints >= Order) and (NumKnots = NumCtrlPoints + Order).

Dim for each curve in VDim specifies the dimension of each CtrlPointDbl set in VCtrlPointDbls. This method expects 2D-polynomial (X,Y) or 2D-rational (X,Y,Weight) curves to be passed as trimming curves. However, you can set a flag so that this method accepts 3D-polynomial (X,Y,Z) or 3D-rational (X,Y,Z,Weight) trim curves. To do this, negate the absolute value of the first value in the VDim array. For example, if the first VDim value is 3, set it to -3. When you do this, 3D trim curves are expected.

If Dim is:

* 2, specify (X,Y) control points in each CtrlPointDbl set.* -2, specify (X,Y,Z) control points in each CtrlPointDbl set.* 3, specify (X,Y,Weight) control points in each CtrlPointDbl.* -3, specify (X,Y,Z,Weight) control points in each CtrlPointDbl.

Multiplicity of a knot is the number of times it is repeated in the knot vector. There are specific rules around number of knots, knot multiplicity, and curve order. For example, if a curve's Periodic value is:

* 0 (non-periodic), there must be (NumCtrlPoints + Order) knots and the maximum multiplicity of any knot is Order.* 1 (periodic), there must be (NumCtrlPoints + 1) knots and the maximum multiplicity of any knot is Order. If a knot has multiplicity greater than 1, repetitions must occur at the end of the knot vector.

If you do not want to specify a UV range, use null or Nothing in the UvRange array elements.

After calling this method to add a trimming loop, you can generate the trimmed surface by calling [IBody2::CreateTrimmedSurface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~CreateTrimmedSurface.html). You can create a body from trimmed surfaces using [IBody2::CreateBodyFromSurfaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateBodyFromSurfaces.html).

NOTE: It is highly recommended that you consult other resources for the mathematics behind b-splines, knots, knot multiplicity, and control points before attempting to use this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)

[ISurface::IAddTrimmingLoop2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IAddTrimmingLoop2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0