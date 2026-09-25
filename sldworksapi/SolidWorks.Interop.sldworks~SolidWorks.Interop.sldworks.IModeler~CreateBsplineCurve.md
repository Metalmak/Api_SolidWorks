<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateBsplineCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateBsplineCurve Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : CreateBsplineCurve Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Props*
:   Array containing 4 integers packed into 2 double elements (see **Remarks**)

*Knots*
:   Array of numKnots doubles (see Remarks)

*CtrlPtCoords*
:   Array of NumCtrlPtCoord doubles (see Remarks)

Creates a b-spline curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateBsplineCurve( _    ByVal Props As System.Object, _    ByVal Knots As System.Object, _    ByVal CtrlPtCoords As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Props As System.Object Dim Knots As System.Object Dim CtrlPtCoords As System.Object Dim value As System.Object   value = instance.CreateBsplineCurve(Props, Knots, CtrlPtCoords) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateBsplineCurve(     System.object Props,    System.object Knots,    System.object CtrlPtCoords ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateBsplineCurve(  &   System.Object^ Props, &   System.Object^ Knots, &   System.Object^ CtrlPtCoords ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Props*
:   Array containing 4 integers packed into 2 double elements (see **Remarks**)

*Knots*
:   Array of numKnots doubles (see Remarks)

*CtrlPtCoords*
:   Array of NumCtrlPtCoord doubles (see Remarks)

#### Return Value

B-spline [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::CreateBsplineCurve.

# ![](dotnetimages/collapse.gif)Remarks

The Props argument contains the following values:

* DimensionControlPoints

  * Order

    * NumCtrlPoints

      * Periodicity

|  |  |
| --- | --- |
| **Length of this array...** | **Given by...** |
| Knots | numKnots = NumCtrlPoints + Order |
| CtrlPtCoords | NumCtrlPtCoord = NumCtrlPoints + DimensionControlPoints |

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::ICreateBsplineCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateBsplineCurve.html)

[IBody2::AddProfileBspline Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~AddProfileBspline.html)

[IBody2::IAddProfileBspline Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddProfileBspline.html)