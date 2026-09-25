<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace~IGetFacetData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetFacetData Method (IFace) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFace Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace.html) : IGetFacetData Method (IFace) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FacetMesh*

*NFacets*

*NStrips*

*StripVertexNums*

*VertexCoords*

*NormalCoords*

Obsolete. Superseded by [IFace2::IGetTessNorms](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~IGetTessNorms.html), [IFace2::IGetTessTextures](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~IGetTessTextures.html), [IFace2::GetTessTriangleCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~GetTessTriangleCount.html), [IFace2::IGetTriangles](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~IGetTessTriangles.html), [IFace2::IGetTessTriStripEdges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~IGetTessTriStripEdges.html), [IFace2::IGetTessTriStrips](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~IGetTessTriStrips.html), and [IFace2::GetTessTriStripSize](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~GetTessTriStripSize.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IGetFacetData( _    ByVal FacetMesh As System.Integer, _    ByRef NFacets As System.Integer, _    ByRef NStrips As System.Integer, _    ByVal StripVertexNums As System.IntPtr, _    ByVal VertexCoords As System.IntPtr, _    ByVal NormalCoords As System.IntPtr _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFace Dim FacetMesh As System.Integer Dim NFacets As System.Integer Dim NStrips As System.Integer Dim StripVertexNums As System.IntPtr Dim VertexCoords As System.IntPtr Dim NormalCoords As System.IntPtr   instance.IGetFacetData(FacetMesh, NFacets, NStrips, StripVertexNums, VertexCoords, NormalCoords) ``` | |

| C# |  |
| --- | --- |
| ``` void IGetFacetData(     System.int FacetMesh,    ref System.int NFacets,    ref System.int NStrips,    System.IntPtr StripVertexNums,    System.IntPtr VertexCoords,    System.IntPtr NormalCoords ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IGetFacetData(  &   System.int FacetMesh, &   System.int% NFacets, &   System.int% NStrips, &   System.IntPtr StripVertexNums, &   System.IntPtr VertexCoords, &   System.IntPtr NormalCoords ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FacetMesh*

*NFacets*

*NStrips*

*StripVertexNums*

*VertexCoords*

*NormalCoords*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Face::IGetFacetData.

# ![](dotnetimages/collapse.gif)See Also

####

[IFace Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace.html)

[IFace Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace_members.html)