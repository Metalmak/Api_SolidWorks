<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreatePCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreatePCurve Method (IModeler) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : CreatePCurve Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Surface*
:   [Surface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface.html) associated with the pcurve

*Props*
:   Array containing 4 integers packed into 2 double elements (see **Remarks**)

*Knots*
:   Array of numKnots (see **Remarks**)

*CtrlPtCoords*
:   Array of numCtrlPtCoord (see **Remarks**)

Creates a pcurve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreatePCurve( _    ByVal Surface As System.Object, _    ByVal Props As System.Object, _    ByVal Knots As System.Object, _    ByVal CtrlPtCoords As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Surface As System.Object Dim Props As System.Object Dim Knots As System.Object Dim CtrlPtCoords As System.Object Dim value As System.Object   value = instance.CreatePCurve(Surface, Props, Knots, CtrlPtCoords) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreatePCurve(     System.object Surface,    System.object Props,    System.object Knots,    System.object CtrlPtCoords ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreatePCurve(  &   System.Object^ Surface, &   System.Object^ Props, &   System.Object^ Knots, &   System.Object^ CtrlPtCoords ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Surface*
:   [Surface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface.html) associated with the pcurve

*Props*
:   Array containing 4 integers packed into 2 double elements (see **Remarks**)

*Knots*
:   Array of numKnots (see **Remarks**)

*CtrlPtCoords*
:   Array of numCtrlPtCoord (see **Remarks**)

#### Return Value

[Pcurve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::CreatePCurve.

# ![](dotnetimages/collapse.gif)Example

[Create Space Parameter Curve On Surface (VBA)](Create_Space_Parameter_Curve_on_Surface_Example_VB.htm)

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
| CtrlPtCoords | NumCtrlPtCoord = NumCtrlPoints \* DimensionControlPoints |

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::ICreatePCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreatePCurve.html)

[ICurve::GetPCurveParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~GetPCurveParams.html)

[ICurve::IGetPCurveParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IGetPCurveParams.html)

[ICurve::IGetPCurveParamsSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IGetPCurveParamsSize.html)

[IModeler::CreateBsplineCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateBsplineCurve.html)

[IModeler::ICreateBsplineCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateBsplineCurve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0