<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~IImprintCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IImprintCurve Method (IFace2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFace2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) : IImprintCurve Method (IFace2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Curve*
:   Pointer to the [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html) to imprint on the face

*NewEdgeCount*
:   Number of new edges to create

*NewEdges*
:   Array of new [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) created by the imprinted curve of size NewEdgeCount

*NewFaceCount*
:   Number of new faces to create

*NewFaces*
:   Array of new [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) created by the imprinted curve of size NewFaceCount

Imprints a curve on the selected face.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IImprintCurve( _    ByVal Curve As Curve, _    ByVal NewEdgeCount As System.Integer, _    ByRef NewEdges As Edge, _    ByVal NewFaceCount As System.Integer, _    ByRef NewFaces As Face2 _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFace2 Dim Curve As Curve Dim NewEdgeCount As System.Integer Dim NewEdges As Edge Dim NewFaceCount As System.Integer Dim NewFaces As Face2   instance.IImprintCurve(Curve, NewEdgeCount, NewEdges, NewFaceCount, NewFaces) ``` | |

| C# |  |
| --- | --- |
| ``` void IImprintCurve(     Curve Curve,    System.int NewEdgeCount,    out Edge NewEdges,    System.int NewFaceCount,    out Face2 NewFaces ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IImprintCurve(  &   Curve^ Curve, &   System.int NewEdgeCount, &   [Out] Edge^ NewEdges, &   System.int NewFaceCount, &   [Out] Face2^ NewFaces ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Curve*
:   Pointer to the [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html) to imprint on the face

*NewEdgeCount*
:   Number of new edges to create

*NewEdges*
:   Array of new [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) created by the imprinted curve of size NewEdgeCount

*NewFaceCount*
:   Number of new faces to create

*NewFaces*
:   Array of new [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) created by the imprinted curve of size NewFaceCount

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Face2::IImprintCurve.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IFace2::ImprintCurveCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~ImprintCurveCount.html) to get the size of the arrays.

The specified curve must lie on the face.

To imprint a curve on a new face of a temporary body, create a copy of the original curve and imprint the copy of the curve on the new face.

# ![](dotnetimages/collapse.gif)See Also

####

[IFace2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)

[IFace2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2_members.html)

[IFace2::ImprintCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~ImprintCurve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP2, Revision Number 12.2