<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~IImprintingFaces.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IImprintingFaces Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : IImprintingFaces Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TargetEdges*
:   Array of target [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html)

*ToolEdges*
:   Array of tool [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html)

*TargetVertices*
:   Array of target [vertices](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IVertex.html)

*ToolVertices*
:   Array of tool [vertices](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IVertex.html)

Imprints the specified tool faces onto the specified target faces.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IImprintingFaces( _    ByRef TargetEdges As Edge, _    ByRef ToolEdges As Edge, _    ByRef TargetVertices As Vertex, _    ByRef ToolVertices As Vertex _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim TargetEdges As Edge Dim ToolEdges As Edge Dim TargetVertices As Vertex Dim ToolVertices As Vertex   instance.IImprintingFaces(TargetEdges, ToolEdges, TargetVertices, ToolVertices) ``` | |

| C# |  |
| --- | --- |
| ``` void IImprintingFaces(     out Edge TargetEdges,    out Edge ToolEdges,    out Vertex TargetVertices,    out Vertex ToolVertices ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IImprintingFaces(  &   [Out] Edge^ TargetEdges, &   [Out] Edge^ ToolEdges, &   [Out] Vertex^ TargetVertices, &   [Out] Vertex^ ToolVertices ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TargetEdges*
:   Array of target [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html)

*ToolEdges*
:   Array of tool [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html)

*TargetVertices*
:   Array of target [vertices](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IVertex.html)

*ToolVertices*
:   Array of tool [vertices](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IVertex.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::IImprintingFaces.

# ![](dotnetimages/collapse.gif)Remarks

Call [IModeler::IImprintingFacesCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~IImprintingFacesCount2.html) before calling this method.

The target and tool faces must:

* belong to different bodies.

  * intersect each other.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::ImprintingFaces Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ImprintingFaces.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0