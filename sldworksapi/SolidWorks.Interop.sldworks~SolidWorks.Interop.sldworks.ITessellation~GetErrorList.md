<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetErrorList.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetErrorList Method (ITessellation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITessellation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation.html) : GetErrorList Method (ITessellation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FaceErrArray*
:   Array of tessellation faces that have errors

*FacetErrArray*
:   Array of tessellation facets that have errors

*VertexPointErrArray*
:   Array of tessellation vertex points that have errors

*VertexNormalErrArray*
:   Array of tessellation vertex normals that have errors

*VertexParamsErrArray*
:   Array of tessellation vertex parameters that have errors

Gets the tessellation error list.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetErrorList( _    ByRef FaceErrArray As System.Object, _    ByRef FacetErrArray As System.Object, _    ByRef VertexPointErrArray As System.Object, _    ByRef VertexNormalErrArray As System.Object, _    ByRef VertexParamsErrArray As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITessellation Dim FaceErrArray As System.Object Dim FacetErrArray As System.Object Dim VertexPointErrArray As System.Object Dim VertexNormalErrArray As System.Object Dim VertexParamsErrArray As System.Object   instance.GetErrorList(FaceErrArray, FacetErrArray, VertexPointErrArray, VertexNormalErrArray, VertexParamsErrArray) ``` | |

| C# |  |
| --- | --- |
| ``` void GetErrorList(     out System.object FaceErrArray,    out System.object FacetErrArray,    out System.object VertexPointErrArray,    out System.object VertexNormalErrArray,    out System.object VertexParamsErrArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetErrorList(  &   [Out] System.Object^ FaceErrArray, &   [Out] System.Object^ FacetErrArray, &   [Out] System.Object^ VertexPointErrArray, &   [Out] System.Object^ VertexNormalErrArray, &   [Out] System.Object^ VertexParamsErrArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FaceErrArray*
:   Array of tessellation faces that have errors

*FacetErrArray*
:   Array of tessellation facets that have errors

*VertexPointErrArray*
:   Array of tessellation vertex points that have errors

*VertexNormalErrArray*
:   Array of tessellation vertex normals that have errors

*VertexParamsErrArray*
:   Array of tessellation vertex parameters that have errors

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Tessellation::GetErrorList.

# ![](dotnetimages/collapse.gif)Remarks

Before using this method, make sure that you can retrieve the list for the tessellation data that you want to query error information from:

* [ITessellation::NeedVertexNormal](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITessellation~NeedVertexNormal.html)

  * [ITessellation::NeedVertexParams](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITessellation~NeedVertexParams.html)

    * [ITessellation::NeedFaceFacetMap](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITessellation~NeedFaceFacetMap.html)

      * [ITessellation::NeedEdgeFinMap](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITessellation~NeedEdgeFinMap.html)

        * [ITessellation::NeedErrorList](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITessellation~NeedErrorList.html)

After using an ITessellation function, you can return error information about any of the tessellation data.

The arrays returned by ITessellation::GetErrorList contains the tessellation entity IDs that have errors:

* Face error: The specified face could not be faceted.

  * Facet error: The specified facet is disconnected from its neighboring facets.

    * Vertex error: The specified vertex does not match any vertices on adjacent faces. There may be gaps between facets.

      * Vertex normal error: The tessellate function could not calculate an accurate vertex normal.

        * Vertex parameter error: The tessellate function could not calculate accurate vertex parameters.

# ![](dotnetimages/collapse.gif)See Also

####

[ITessellation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation.html)

[ITessellation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation_members.html)

[ITessellation::IGetErrorList2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetErrorList2.html)

[ITessellation::IGetErrorListCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetErrorListCount.html)

[ITessellate::NeedErrorList Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~NeedErrorList.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0