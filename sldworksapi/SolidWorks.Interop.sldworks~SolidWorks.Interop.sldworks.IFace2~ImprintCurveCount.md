<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~ImprintCurveCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ImprintCurveCount Method (IFace2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFace2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) : ImprintCurveCount Method (IFace2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Curve*
:   Pointer to the [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

*NewEdgeCount*
:   Number of new edges to create when imprinting this curve

*NewFaceCount*
:   Number of new faces to create when imprinting this curve

Gets the number of new edges and faces to create when imprinting a curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ImprintCurveCount( _    ByVal Curve As Curve, _    ByRef NewEdgeCount As System.Integer, _    ByRef NewFaceCount As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFace2 Dim Curve As Curve Dim NewEdgeCount As System.Integer Dim NewFaceCount As System.Integer   instance.ImprintCurveCount(Curve, NewEdgeCount, NewFaceCount) ``` | |

| C# |  |
| --- | --- |
| ``` void ImprintCurveCount(     Curve Curve,    out System.int NewEdgeCount,    out System.int NewFaceCount ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ImprintCurveCount(  &   Curve^ Curve, &   [Out] System.int NewEdgeCount, &   [Out] System.int NewFaceCount ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Curve*
:   Pointer to the [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

*NewEdgeCount*
:   Number of new edges to create when imprinting this curve

*NewFaceCount*
:   Number of new faces to create when imprinting this curve

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Face2::ImprintCurveCount.

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [IFace2::IImprintCurve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~IImprintCurve.html) to get the size of the edges and faces arrays.

# ![](dotnetimages/collapse.gif)See Also

####

[IFace2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)

[IFace2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2_members.html)

[IFace2::ImprintCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~ImprintCurve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP2, Revision Number 12.2