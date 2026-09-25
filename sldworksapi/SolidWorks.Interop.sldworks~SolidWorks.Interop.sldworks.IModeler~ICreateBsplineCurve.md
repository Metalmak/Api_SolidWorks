<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateBsplineCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateBsplineCurve Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ICreateBsplineCurve Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Properties*
:   Array containing 4 integers packed into 2 double elements (see **Remarks**)

*KnotArray*
:   Array of numKnots doubles (see Remarks)

*ControlPointCoordArray*
:   Array of NumCtrlPtCoord doubles (see Remarks)

Creates a b-spline curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateBsplineCurve( _    ByRef Properties As System.Integer, _    ByRef KnotArray As System.Double, _    ByRef ControlPointCoordArray As System.Double _ ) As Curve ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Properties As System.Integer Dim KnotArray As System.Double Dim ControlPointCoordArray As System.Double Dim value As Curve   value = instance.ICreateBsplineCurve(Properties, KnotArray, ControlPointCoordArray) ``` | |

| C# |  |
| --- | --- |
| ``` Curve ICreateBsplineCurve(     ref System.int Properties,    ref System.double KnotArray,    ref System.double ControlPointCoordArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Curve^ ICreateBsplineCurve(  &   System.int% Properties, &   System.double% KnotArray, &   System.double% ControlPointCoordArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Properties*
:   Array containing 4 integers packed into 2 double elements (see **Remarks**)

*KnotArray*
:   Array of numKnots doubles (see Remarks)

*ControlPointCoordArray*
:   Array of NumCtrlPtCoord doubles (see Remarks)

#### Return Value

B-spline [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ICreateBsplineCurve.

# ![](dotnetimages/collapse.gif)Remarks

The Properties argument contains the following values:

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

[IModeler::CreateBsplineCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateBsplineCurve.html)

[IModeler::CreateBsplineSurface Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateBsplineSurface.html)

[IModeler::ICreateBsplineSurface Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateBsplineSurface.html)