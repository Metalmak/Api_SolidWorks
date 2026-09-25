<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~Evaluate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Evaluate Method (IEdge) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEdge Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html) : Evaluate Method (IEdge) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Parameter*
:   Value of the edge parameter

Obsolete. Superseded by [IEdge::Evaluate2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~Evaluate2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Evaluate( _    ByVal Parameter As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEdge Dim Parameter As System.Double Dim value As System.Object   value = instance.Evaluate(Parameter) ``` | |

| C# |  |
| --- | --- |
| ``` System.object Evaluate(     System.double Parameter ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ Evaluate(  &   System.double Parameter ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Parameter*
:   Value of the edge parameter

#### Return Value

Array values containing the x,y,z value and derivative of the edge (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Edge::Evaluate.

# ![](dotnetimages/collapse.gif)Example

[Select Tangent Edges Via Iteration (VBA)](Select_Tangent_Edges_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use [IEdge::GetCurveParams2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~GetCurveParams2.html) or [IEdge::IGetCurveParams2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~IEvaluate.html) to determine the valid parameter range for this method.

This OLE implementation of this method returns an array of doubles as follows:

[ PointX, PointY, PointZ, TangentX, TangentY, TangentZ, Success ]

where the point values are in meters and Success is True if successful and false if not.

The return value for the COM implementation is different. To determine success, check the HRESULT return value. The array is as follows:

[ PointX, PointY, PointZ, TangentX, TangentY, TangentZ ]

where the point values are specified in meters.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdge Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html)

[IEdge Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge_members.html)

[IEdge::IEvaluate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IEvaluate.html)