<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~IImprintingFacesCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IImprintingFacesCount Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : IImprintingFacesCount Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NTargetFaces*

*TargetFaceArray*

*NToolFaces*

*ToolFaceArray*

*Options*

*NTargetEdges*

*NtoolEdges*

*NtargetVertices*

*ToolVertices*

Obsolete. Superseded by [IModeler::IImprintingFacesCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~IImprintingFacesCount2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IImprintingFacesCount( _    ByVal NTargetFaces As System.Integer, _    ByRef TargetFaceArray As Face, _    ByVal NToolFaces As System.Integer, _    ByRef ToolFaceArray As Face, _    ByVal Options As System.Integer, _    ByRef NTargetEdges As System.Integer, _    ByRef NtoolEdges As System.Integer, _    ByRef NtargetVertices As System.Integer, _    ByRef ToolVertices As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim NTargetFaces As System.Integer Dim TargetFaceArray As Face Dim NToolFaces As System.Integer Dim ToolFaceArray As Face Dim Options As System.Integer Dim NTargetEdges As System.Integer Dim NtoolEdges As System.Integer Dim NtargetVertices As System.Integer Dim ToolVertices As System.Integer Dim value As System.Boolean   value = instance.IImprintingFacesCount(NTargetFaces, TargetFaceArray, NToolFaces, ToolFaceArray, Options, NTargetEdges, NtoolEdges, NtargetVertices, ToolVertices) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IImprintingFacesCount(     System.int NTargetFaces,    ref Face TargetFaceArray,    System.int NToolFaces,    ref Face ToolFaceArray,    System.int Options,    out System.int NTargetEdges,    out System.int NtoolEdges,    out System.int NtargetVertices,    out System.int ToolVertices ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IImprintingFacesCount(  &   System.int NTargetFaces, &   Face^% TargetFaceArray, &   System.int NToolFaces, &   Face^% ToolFaceArray, &   System.int Options, &   [Out] System.int NTargetEdges, &   [Out] System.int NtoolEdges, &   [Out] System.int NtargetVertices, &   [Out] System.int ToolVertices ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NTargetFaces*

*TargetFaceArray*

*NToolFaces*

*ToolFaceArray*

*Options*

*NTargetEdges*

*NtoolEdges*

*NtargetVertices*

*ToolVertices*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::IImprintingFacesCount.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)