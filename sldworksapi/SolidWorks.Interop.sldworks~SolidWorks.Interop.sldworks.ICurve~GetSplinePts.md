<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~GetSplinePts.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSplinePts Method (ICurve) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : GetSplinePts Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ParamsArrayIn*
:   Array containing the definition of the spline

Gets the spline points for this curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSplinePts( _    ByVal ParamsArrayIn As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim ParamsArrayIn As System.Object Dim value As System.Object   value = instance.GetSplinePts(ParamsArrayIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetSplinePts(     System.object ParamsArrayIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetSplinePts(  &   System.Object^ ParamsArrayIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ParamsArrayIn*
:   Array containing the definition of the spline

#### Return Value

Array containing the spline points

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::GetSplinePts.

# ![](dotnetimages/collapse.gif)Example

[Get Curve Spline Points (VBA)](Get_Curve_Spline_Points_Example_VB.htm)

[Get Length of Spline or Elliptical Edge (VBA)](Get_Length_of_Spline_or_Elliptical_Edge_Example_VB.htm)

[Get Parameters and Spline Points for Curve (VBA)](Get_Parameters_and_Spline_Points_for_Curve_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

For OLE Automation applications, the ParamsIn argument contains an array defining the spline. This array contains the values for propArray, knotsArray and cntrlPntCoordArray, all packed into a single array (propArray is packed as four integers into the first two elements of the array.) The contents of these arrays is described in [ICurve::IGetSplinePtsSize](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IGetSplinePtsSize.html).

The array returned contains the x, y, z location of the spline points:

> **[** *x1, y1, z1, x2, y2, z2*,....**]**

Data passed into this method must satisfy the following requirements:

* If the curve is periodic, it must not have any repeated knots.* If the curve is non-periodic, it must only have repeated knots at its ends.* The curve must be cubic or lower degree, non-rational, and have continuous first
      and second derivatives.

**NOTE:** For a linear or quadratic curve to satisfy these continuity requirements, it must consist of a single segment.

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::IGetSplinePts Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IGetSplinePts.html)