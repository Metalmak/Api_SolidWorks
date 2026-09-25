<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetErrorListCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetErrorListCount Method (ITessellation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITessellation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation.html) : IGetErrorListCount Method (ITessellation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FaceErrArrayCount*
:   Number of face errors

*FacetErrArrayCount*
:   Number of facet errors

*VertexPointErrArrayCount*
:   Number of vertex point errors

*VertexNormalErrArrayCount*
:   Number of vertex point errors

*VertexParamsErrArrayCount*
:   Number of vertex parameter errors

Gets number of tessellation errors by error type.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IGetErrorListCount( _    ByRef FaceErrArrayCount As System.Integer, _    ByRef FacetErrArrayCount As System.Integer, _    ByRef VertexPointErrArrayCount As System.Integer, _    ByRef VertexNormalErrArrayCount As System.Integer, _    ByRef VertexParamsErrArrayCount As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITessellation Dim FaceErrArrayCount As System.Integer Dim FacetErrArrayCount As System.Integer Dim VertexPointErrArrayCount As System.Integer Dim VertexNormalErrArrayCount As System.Integer Dim VertexParamsErrArrayCount As System.Integer   instance.IGetErrorListCount(FaceErrArrayCount, FacetErrArrayCount, VertexPointErrArrayCount, VertexNormalErrArrayCount, VertexParamsErrArrayCount) ``` | |

| C# |  |
| --- | --- |
| ``` void IGetErrorListCount(     out System.int FaceErrArrayCount,    out System.int FacetErrArrayCount,    out System.int VertexPointErrArrayCount,    out System.int VertexNormalErrArrayCount,    out System.int VertexParamsErrArrayCount ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IGetErrorListCount(  &   [Out] System.int FaceErrArrayCount, &   [Out] System.int FacetErrArrayCount, &   [Out] System.int VertexPointErrArrayCount, &   [Out] System.int VertexNormalErrArrayCount, &   [Out] System.int VertexParamsErrArrayCount ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FaceErrArrayCount*
:   Number of face errors

*FacetErrArrayCount*
:   Number of facet errors

*VertexPointErrArrayCount*
:   Number of vertex point errors

*VertexNormalErrArrayCount*
:   Number of vertex point errors

*VertexParamsErrArrayCount*
:   Number of vertex parameter errors

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Tessellation::IGetErrorListCount.

# ![](dotnetimages/collapse.gif)See Also

####

[ITessellation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation.html)

[ITessellation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation_members.html)

[ITessellation::IGetErrorList2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetErrorList2.html)

[ITessellation::GetErrorList Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetErrorList.html)

[ITessellate::NeedErrorList Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~NeedErrorList.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0