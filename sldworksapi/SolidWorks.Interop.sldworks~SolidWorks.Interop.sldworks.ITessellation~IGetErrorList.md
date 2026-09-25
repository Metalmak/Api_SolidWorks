<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetErrorList.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetErrorList Method (ITessellation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITessellation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation.html) : IGetErrorList Method (ITessellation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FaceErrArray*

*FacetErrArray*

*VertexPointErrArray*

*VertexNormalErrArray*

*VertexParamsErrArray*

Obsolete. Superseded by [ITessellation::IGetErrorList2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITessellation~IGetErrorList2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IGetErrorList( _    ByRef FaceErrArray As Face, _    ByRef FacetErrArray As System.Integer, _    ByRef VertexPointErrArray As System.Integer, _    ByRef VertexNormalErrArray As System.Integer, _    ByRef VertexParamsErrArray As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITessellation Dim FaceErrArray As Face Dim FacetErrArray As System.Integer Dim VertexPointErrArray As System.Integer Dim VertexNormalErrArray As System.Integer Dim VertexParamsErrArray As System.Integer   instance.IGetErrorList(FaceErrArray, FacetErrArray, VertexPointErrArray, VertexNormalErrArray, VertexParamsErrArray) ``` | |

| C# |  |
| --- | --- |
| ``` void IGetErrorList(     out Face FaceErrArray,    out System.int FacetErrArray,    out System.int VertexPointErrArray,    out System.int VertexNormalErrArray,    out System.int VertexParamsErrArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IGetErrorList(  &   [Out] Face^ FaceErrArray, &   [Out] System.int FacetErrArray, &   [Out] System.int VertexPointErrArray, &   [Out] System.int VertexNormalErrArray, &   [Out] System.int VertexParamsErrArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FaceErrArray*

*FacetErrArray*

*VertexPointErrArray*

*VertexNormalErrArray*

*VertexParamsErrArray*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Tessellation::IGetErrorList.

# ![](dotnetimages/collapse.gif)See Also

####

[ITessellation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation.html)

[ITessellation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation_members.html)