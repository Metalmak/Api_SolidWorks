<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdgePoint~GetPointCoordinates.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetPointCoordinates Method (IEdgePoint) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEdgePoint Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdgePoint.html) : GetPointCoordinates Method (IEdgePoint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   x coordinate for this midpoint or endpoint

*Y*
:   y coordinate for this midpoint or endpoint

*Z*
:   z coordinate for this midpoint or endpoint

Gets the coordinates for this midpoint on an [edge](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) or an endpoint or midpoint on a [reference curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IReferenceCurve.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetPointCoordinates( _    ByRef X As System.Double, _    ByRef Y As System.Double, _    ByRef Z As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEdgePoint Dim X As System.Double Dim Y As System.Double Dim Z As System.Double   instance.GetPointCoordinates(X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` void GetPointCoordinates(     out System.double X,    out System.double Y,    out System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetPointCoordinates(  &   [Out] System.double X, &   [Out] System.double Y, &   [Out] System.double Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   x coordinate for this midpoint or endpoint

*Y*
:   y coordinate for this midpoint or endpoint

*Z*
:   z coordinate for this midpoint or endpoint

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EdgePoint::GetPointCoordinates.

# ![](dotnetimages/collapse.gif)Example

[Create Reference Curve (C#)](Create_Reference_Curve_Example_CSharp.htm)

[Create Reference Curve (VB.NET)](Create_Reference_Curve_Example_VBNET.htm)

[Create Reference Curve (VBA)](Create_Reference_Curve_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdgePoint Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdgePoint.html)

[IEdgePoint Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdgePoint_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0