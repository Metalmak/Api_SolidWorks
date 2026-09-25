<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IGetSplinePtsSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetSplinePtsSize Method (ICurve) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : IGetSplinePtsSize Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PropArray*
:   Array that includes dimension, order, number of control points, and periodicity

*KnotsArray*
:   knot1, knot2, ..., knot*n*

*CntrlPntCoordArray*
:   controlpoint1[dimension], controlpoint2[dimension], ...,  controlpoint*n*[dimension]

Gets the size of the array required by [ICurve::IGetSplinePts](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IGetSplinePts.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetSplinePtsSize( _    ByRef PropArray As System.Integer, _    ByRef KnotsArray As System.Double, _    ByRef CntrlPntCoordArray As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim PropArray As System.Integer Dim KnotsArray As System.Double Dim CntrlPntCoordArray As System.Double Dim value As System.Integer   value = instance.IGetSplinePtsSize(PropArray, KnotsArray, CntrlPntCoordArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetSplinePtsSize(     ref System.int PropArray,    ref System.double KnotsArray,    ref System.double CntrlPntCoordArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetSplinePtsSize(  &   System.int% PropArray, &   System.double% KnotsArray, &   System.double% CntrlPntCoordArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PropArray*
:   Array that includes dimension, order, number of control points, and periodicity

*KnotsArray*
:   knot1, knot2, ..., knot*n*

*CntrlPntCoordArray*
:   controlpoint1[dimension], controlpoint2[dimension], ...,  controlpoint*n*[dimension]

#### Return Value

Size of the data set returned by [ICurve::IGetSplinePts](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IGetSplinePts.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::IGetSplinePtsSize.

# ![](dotnetimages/collapse.gif)Example

[Get Curve Spline Points (C++)](Get_Curve_Spline_Points_Example_CPlusPlus_COM.htm)

# ![](dotnetimages/collapse.gif)Remarks

PropArray contains 4 integers:

* Dimension* Order* Number of control points* Periodicity ( True or false )

KnotsArray is an array of doubles with (Number of control points + Order) elements.

The size of the CntrlPntCoordArray array is based on the curve dimension.

* Dimension = 2 then each control point is an array of 2 doubles ( u, v )* Dimension = 3 then each control point is an array of 3 doubles ( x, y, z)* Dimension = 4 then each control point is an array of 4 doubles ( x, y, z, w ) where w = weight

Data passed into this method must satisfy the following requirements:

* If the curve is periodic, it must not have any repeated knots.* If the curve is non-periodic, it must only have repeated knots at its ends.* The curve must be cubic or lower degree, non-rational and have continuous first and second derivatives.

**NOTE:** For a linear or quadratic curve to satisfy these continuity requirements, it
must consist of a single segment.

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::GetSplinePts Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~GetSplinePts.html)