<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddProfileBsplineDLL.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAddProfileBsplineDLL Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : IAddProfileBsplineDLL Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Properties*
:   Contains 4 longs (see **Remarks**)

*KnotArray*
:   Pointer to an array of numKnots doubles (see **Remarks**)

*ControlPointCoordArray*
:   Pointer to an array of numCtrlPtCoord doubles (see **Remarks**)

Adds a profile B-spline.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IAddProfileBsplineDLL( _    ByRef Properties As System.Integer, _    ByRef KnotArray As System.Double, _    ByRef ControlPointCoordArray As System.Double _ ) As Curve ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim Properties As System.Integer Dim KnotArray As System.Double Dim ControlPointCoordArray As System.Double Dim value As Curve   value = instance.IAddProfileBsplineDLL(Properties, KnotArray, ControlPointCoordArray) ``` | |

| C# |  |
| --- | --- |
| ``` Curve IAddProfileBsplineDLL(     ref System.int Properties,    ref System.double KnotArray,    ref System.double ControlPointCoordArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Curve^ IAddProfileBsplineDLL(  &   System.int% Properties, &   System.double% KnotArray, &   System.double% ControlPointCoordArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Properties*
:   Contains 4 longs (see **Remarks**)

*KnotArray*
:   Pointer to an array of numKnots doubles (see **Remarks**)

*ControlPointCoordArray*
:   Pointer to an array of numCtrlPtCoord doubles (see **Remarks**)

#### Return Value

Pointer to the profile B-spline [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::IAddProfileBsplineDLL.

# ![](dotnetimages/collapse.gif)Remarks

You can use this method with [IBody2::ICreateRevolutionSurface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ICreateRevolutionSurface.html) to generate any surface
of revolution or with [IBody2::ICreateExtrusionSurface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ICreateExtrusionSurface.html) to generate a tabulated cylinder.

The Properties argument contains the following values:

* DimensionControlPoints* Order* NumCtrlPoints* Periodicity

The length of the KnotArray argument is:

> numKnots = NumCtrlPoints + Order

The length of the ControlPointCoordArray is:

> numCtrlPtCoord = NumCtrlPoints \* DimensionControlPoints

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0