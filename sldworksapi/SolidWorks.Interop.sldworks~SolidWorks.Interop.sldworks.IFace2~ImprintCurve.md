<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~ImprintCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ImprintCurve Method (IFace2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFace2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) : ImprintCurve Method (IFace2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Curve*
:   [Curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html) to imprint on the face

*NewEdges*
:   Array of new [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) created by the imprinted curve

*NewFaces*
:   Array of new [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) created by the imprinted curve

Imprints a curve on the selected face.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ImprintCurve( _    ByVal Curve As System.Object, _    ByRef NewEdges As System.Object, _    ByRef NewFaces As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFace2 Dim Curve As System.Object Dim NewEdges As System.Object Dim NewFaces As System.Object   instance.ImprintCurve(Curve, NewEdges, NewFaces) ``` | |

| C# |  |
| --- | --- |
| ``` void ImprintCurve(     System.object Curve,    out System.object NewEdges,    out System.object NewFaces ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ImprintCurve(  &   System.Object^ Curve, &   [Out] System.Object^ NewEdges, &   [Out] System.Object^ NewFaces ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Curve*
:   [Curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html) to imprint on the face

*NewEdges*
:   Array of new [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) created by the imprinted curve

*NewFaces*
:   Array of new [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) created by the imprinted curve

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Face2::ImprintCurve.

# ![](dotnetimages/collapse.gif)Remarks

The specified curve must lie on the face.

To imprint a curve on a new face of a temporary body, create a copy of the original curve and imprint the copy of the curve on the new face.

# ![](dotnetimages/collapse.gif)See Also

####

[IFace2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)

[IFace2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2_members.html)

[IFace2::IImprintCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~IImprintCurve.html)

[IFace2::ImprintCurveCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~ImprintCurveCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP2, Revision Number 12.2