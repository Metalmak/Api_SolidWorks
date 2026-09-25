<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~AddProfileBspline.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddProfileBspline Method (IBody2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : AddProfileBspline Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Props*
:   Contains 4 integers packed into 2 double elements (see **Remarks**)

*Knots*
:   Array of numKnots (see Remarks)

*CtrlPtCoords*
:   Array of numCtrlPtCoord (see Remarks)

Creates an B-spline profile curve and returns a pointer to that curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddProfileBspline( _    ByVal Props As System.Object, _    ByVal Knots As System.Object, _    ByVal CtrlPtCoords As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim Props As System.Object Dim Knots As System.Object Dim CtrlPtCoords As System.Object Dim value As System.Object   value = instance.AddProfileBspline(Props, Knots, CtrlPtCoords) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddProfileBspline(     System.object Props,    System.object Knots,    System.object CtrlPtCoords ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddProfileBspline(  &   System.Object^ Props, &   System.Object^ Knots, &   System.Object^ CtrlPtCoords ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Props*
:   Contains 4 integers packed into 2 double elements (see **Remarks**)

*Knots*
:   Array of numKnots (see Remarks)

*CtrlPtCoords*
:   Array of numCtrlPtCoord (see Remarks)

#### Return Value

[Curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::AddProfileBspline.

# ![](dotnetimages/collapse.gif)Example

[Create Reference Curve (C#)](Create_Reference_Curve_Example_CSharp.htm)

[Create Reference Curve (VB.NET)](Create_Reference_Curve_Example_VBNET.htm)

[Create Reference Curve (VBA)](Create_Reference_Curve_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can use this method with [IBody2::CreateRevolutionSurface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~CreateRevolutionSurface.html) to generate any surface of revolution or with [IBody2::CreateExtrusionSurface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~CreateExtrusionSurface.html) to generate a tabulated cylinder.

The Props argument contains the following values:

* DimensionControlPoints

  * Order

    * NumCtrlPoints

      * Periodicity

The length of the knots array is given by:

> numKnots = NumCtrlPoints + Order

The length of the CtrlPtCoords is given by:

> NumCtrlPtCoord = NumCtrlPoints + DimensionControlPoints

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::IAddProfileBspline Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddProfileBspline.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0