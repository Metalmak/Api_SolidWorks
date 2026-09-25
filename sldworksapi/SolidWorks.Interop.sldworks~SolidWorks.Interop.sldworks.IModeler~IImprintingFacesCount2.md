<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~IImprintingFacesCount2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IImprintingFacesCount2 Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : IImprintingFacesCount2 Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NTargetFaces*
:   Number of faces in the target body

*TargetFaceArray*
:   Array of the [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that describe the target body

*NToolFaces*
:   Number of faces in the tool body

*ToolFaceArray*
:   Array of the [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that describe the tool body

*Options*
:   Options for this operation as defined in swImprintingFacesOpts\_e

*NTargetEdges*
:   Number of edges returned from this operation

*NtoolEdges*
:   Number of tool edges returned from this operation

*NtargetVertices*
:   Number of target vertices returned from this operation

*ToolVertices*
:   Number of tool vertices returned from this operation

Gets the number of imprinted edges and vertices in the model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IImprintingFacesCount2( _    ByVal NTargetFaces As System.Integer, _    ByRef TargetFaceArray As Face2, _    ByVal NToolFaces As System.Integer, _    ByRef ToolFaceArray As Face2, _    ByVal Options As System.Integer, _    ByRef NTargetEdges As System.Integer, _    ByRef NtoolEdges As System.Integer, _    ByRef NtargetVertices As System.Integer, _    ByRef ToolVertices As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim NTargetFaces As System.Integer Dim TargetFaceArray As Face2 Dim NToolFaces As System.Integer Dim ToolFaceArray As Face2 Dim Options As System.Integer Dim NTargetEdges As System.Integer Dim NtoolEdges As System.Integer Dim NtargetVertices As System.Integer Dim ToolVertices As System.Integer Dim value As System.Boolean   value = instance.IImprintingFacesCount2(NTargetFaces, TargetFaceArray, NToolFaces, ToolFaceArray, Options, NTargetEdges, NtoolEdges, NtargetVertices, ToolVertices) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IImprintingFacesCount2(     System.int NTargetFaces,    ref Face2 TargetFaceArray,    System.int NToolFaces,    ref Face2 ToolFaceArray,    System.int Options,    out System.int NTargetEdges,    out System.int NtoolEdges,    out System.int NtargetVertices,    out System.int ToolVertices ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IImprintingFacesCount2(  &   System.int NTargetFaces, &   Face2^% TargetFaceArray, &   System.int NToolFaces, &   Face2^% ToolFaceArray, &   System.int Options, &   [Out] System.int NTargetEdges, &   [Out] System.int NtoolEdges, &   [Out] System.int NtargetVertices, &   [Out] System.int ToolVertices ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NTargetFaces*
:   Number of faces in the target body

*TargetFaceArray*
:   Array of the [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that describe the target body

*NToolFaces*
:   Number of faces in the tool body

*ToolFaceArray*
:   Array of the [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that describe the tool body

*Options*
:   Options for this operation as defined in swImprintingFacesOpts\_e

*NTargetEdges*
:   Number of edges returned from this operation

*NtoolEdges*
:   Number of tool edges returned from this operation

*NtargetVertices*
:   Number of target vertices returned from this operation

*ToolVertices*
:   Number of tool vertices returned from this operation

#### Return Value

True if the operation is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::IImprintingFacesCount2.

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [IModeler::IImprintingFaces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~IImprintingFaces.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::ImprintingFaces Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ImprintingFaces.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0