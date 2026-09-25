<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ImprintingFaces.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ImprintingFaces Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ImprintingFaces Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TargetFaceArray*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that describe the target body

*ToolFaceArray*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that describe the tool body

*Options*
:   Options for this operation as defined in swImprintingFacesOpts\_e

*TargetEdges*
:   Array target [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html)

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
| ``` Function ImprintingFaces( _    ByVal TargetFaceArray As System.Object, _    ByVal ToolFaceArray As System.Object, _    ByVal Options As System.Integer, _    ByRef TargetEdges As System.Object, _    ByRef ToolEdges As System.Object, _    ByRef TargetVertices As System.Object, _    ByRef ToolVertices As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim TargetFaceArray As System.Object Dim ToolFaceArray As System.Object Dim Options As System.Integer Dim TargetEdges As System.Object Dim ToolEdges As System.Object Dim TargetVertices As System.Object Dim ToolVertices As System.Object Dim value As System.Boolean   value = instance.ImprintingFaces(TargetFaceArray, ToolFaceArray, Options, TargetEdges, ToolEdges, TargetVertices, ToolVertices) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ImprintingFaces(     System.object TargetFaceArray,    System.object ToolFaceArray,    System.int Options,    out System.object TargetEdges,    out System.object ToolEdges,    out System.object TargetVertices,    out System.object ToolVertices ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ImprintingFaces(  &   System.Object^ TargetFaceArray, &   System.Object^ ToolFaceArray, &   System.int Options, &   [Out] System.Object^ TargetEdges, &   [Out] System.Object^ ToolEdges, &   [Out] System.Object^ TargetVertices, &   [Out] System.Object^ ToolVertices ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TargetFaceArray*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that describe the target body

*ToolFaceArray*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that describe the tool body

*Options*
:   Options for this operation as defined in swImprintingFacesOpts\_e

*TargetEdges*
:   Array target [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html)

*ToolEdges*
:   Array of tool [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html)

*TargetVertices*
:   Array of target [vertices](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IVertex.html)

*ToolVertices*
:   Array of tool [vertices](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IVertex.html)

#### Return Value

True if the operation was successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ImprintingFaces.

# ![](dotnetimages/collapse.gif)Remarks

The target and tool faces must:

* belong to different bodies.

  * intersect each other.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::IImprintingFaces Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~IImprintingFaces.html)

[IModeler::IImprintingFacesCount2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~IImprintingFacesCount2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0