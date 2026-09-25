<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ITessellation Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ITessellation Interface |

The following tables list the members exposed by [ITessellation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CurveChordAngleTolerance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~CurveChordAngleTolerance.html) | Gets or sets the maximum angle, in radians, that is allowed between a chord and its originating curve. |
| ![ Property](dotnetimages/Property.gif) | [CurveChordTolerance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~CurveChordTolerance.html) | Gets or sets the maximum permitted distance from a chord (facet fin) to the curve (edge entity). |
| ![ Property](dotnetimages/Property.gif) | [ImprovedQuality](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~ImprovedQuality.html) | Gets or sets whether to return higher-quality data. |
| ![ Property](dotnetimages/Property.gif) | [MatchType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~MatchType.html) | Gets or sets the type of Parasolid facet match for the tessellation. |
| ![ Property](dotnetimages/Property.gif) | [MaxFacetWidth](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~MaxFacetWidth.html) | Gets or sets the maximum width of any side of a facet. |
| ![ Property](dotnetimages/Property.gif) | [MinFacetWidth](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~MinFacetWidth.html) | Gets or sets the minimum facet width for this tessellation. |
| ![ Property](dotnetimages/Property.gif) | [NeedEdgeFinMap](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~NeedEdgeFinMap.html) | Gets or sets the need edge fin map option. |
| ![ Property](dotnetimages/Property.gif) | [NeedErrorList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~NeedErrorList.html) | Gets or sets the need error list option. |
| ![ Property](dotnetimages/Property.gif) | [NeedFaceFacetMap](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~NeedFaceFacetMap.html) | Gets or sets the need face facet map option. |
| ![ Property](dotnetimages/Property.gif) | [NeedVertexNormal](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~NeedVertexNormal.html) | Gets or sets the need vertex normal option. |
| ![ Property](dotnetimages/Property.gif) | [NeedVertexParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~NeedVertexParams.html) | Gets or sets the need vertex params option. |
| ![ Property](dotnetimages/Property.gif) | [SurfacePlaneAngleTolerance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~SurfacePlaneAngleTolerance.html) | Gets or sets the surface plane angle tolerance. |
| ![ Property](dotnetimages/Property.gif) | [SurfacePlaneTolerance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~SurfacePlaneTolerance.html) | Gets or sets the surface plane tolerance. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetEdgeFins](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetEdgeFins.html) | Gets all of the fin IDs corresponding to a edge. |
| ![ Method](dotnetimages/Method.gif) | [GetErrorList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetErrorList.html) | Gets the tessellation error list. |
| ![ Method](dotnetimages/Method.gif) | [GetFaceFacets](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetFaceFacets.html) | Gets the facets IDs that correspond to a SOLIDWORKS face. |
| ![ Method](dotnetimages/Method.gif) | [GetFacetCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetFacetCount.html) | Gets the number of facets used to create this tessellation. |
| ![ Method](dotnetimages/Method.gif) | [GetFacetFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetFacetFace.html) | Gets a face that corresponds to a facet. |
| ![ Method](dotnetimages/Method.gif) | [GetFacetFins](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetFacetFins.html) | Gets all of the fin IDs of the fins that border this facet. |
| ![ Method](dotnetimages/Method.gif) | [GetFinCoFin](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetFinCoFin.html) | Gets the ID of the CoFin that is shared by a fin. |
| ![ Method](dotnetimages/Method.gif) | [GetFinCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetFinCount.html) | Gets the number of fins for this tessellation. |
| ![ Method](dotnetimages/Method.gif) | [GetFinEdge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetFinEdge.html) | Gets the edge corresponding to a fin. |
| ![ Method](dotnetimages/Method.gif) | [GetFinVertices](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetFinVertices.html) | Gets the IDs of the two vertices that correspond to a fin. |
| ![ Method](dotnetimages/Method.gif) | [GetVertexCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetVertexCount.html) | Gets the number of vertices for this tessellation. |
| ![ Method](dotnetimages/Method.gif) | [GetVertexNormal](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetVertexNormal.html) | Gets the information that describes the normal direction corresponding to vertex. |
| ![ Method](dotnetimages/Method.gif) | [GetVertexParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetVertexParams.html) | Gets the parameters corresponding to a tessellation vertex. |
| ![ Method](dotnetimages/Method.gif) | [GetVertexPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetVertexPoint.html) | Gets the X, Y and Z values that describe a tessellation vertex. |
| ![ Method](dotnetimages/Method.gif) | [IGetEdgeFins](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetEdgeFins.html) | Gets all of the fin IDs corresponding to a edge. |
| ![ Method](dotnetimages/Method.gif) | [IGetEdgeFinsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetEdgeFinsCount.html) | Gets the number of fins corresponding to an edge. |
| ![ Method](dotnetimages/Method.gif) | [IGetErrorList](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetErrorList.html) | Obsolete. Superseded by [ITessellation::IGetErrorList2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITessellation~IGetErrorList2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetErrorList2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetErrorList2.html) | Gets the tessellation error list. |
| ![ Method](dotnetimages/Method.gif) | [IGetErrorListCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetErrorListCount.html) | Gets number of tessellation errors by error type. |
| ![ Method](dotnetimages/Method.gif) | [IGetFaceFacets](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetFaceFacets.html) | Obsolete. Superseded by [ITessellation::IGetFaceFacets2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITessellation~IGetFaceFacets2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetFaceFacets2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetFaceFacets2.html) | Gets the facets IDs that correspond to a face. |
| ![ Method](dotnetimages/Method.gif) | [IGetFaceFacetsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetFaceFacetsCount.html) | Obsolete. Superseded by [ITessellation::IGetFaceFacetsCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITessellation~IGetFaceFacetsCount2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetFaceFacetsCount2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetFaceFacetsCount2.html) | Gets the number of facets corresponding to a face. |
| ![ Method](dotnetimages/Method.gif) | [IGetFacetFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetFacetFace.html) | Obsolete. Superseded by [ITessellation::IGetFacetFace2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITessellation~IGetFacetFace2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetFacetFace2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetFacetFace2.html) | Gets a face that corresponds to a facet. |
| ![ Method](dotnetimages/Method.gif) | [IGetFacetFins](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetFacetFins.html) | Gets all of the fin IDs of the fins that border this facet. |
| ![ Method](dotnetimages/Method.gif) | [IGetFacetFinsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetFacetFinsCount.html) | Gets the number of fins corresponding to a facet. |
| ![ Method](dotnetimages/Method.gif) | [IGetFinEdge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetFinEdge.html) | Gets the edge corresponding to a fin. |
| ![ Method](dotnetimages/Method.gif) | [IGetFinVertices](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetFinVertices.html) | Gets the IDs of the two vertices that correspond to a fin. |
| ![ Method](dotnetimages/Method.gif) | [IGetVertexNormal](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetVertexNormal.html) | Gets the information that describes the normal direction corresponding to vertex. |
| ![ Method](dotnetimages/Method.gif) | [IGetVertexParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetVertexParams.html) | Gets the parameters corresponding to a tessellation vertex. |
| ![ Method](dotnetimages/Method.gif) | [IGetVertexPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetVertexPoint.html) | Gets the X, Y and Z values that describe a tessellation vertex. |
| ![ Method](dotnetimages/Method.gif) | [Tessellate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~Tessellate.html) | Performs the tessellation. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ITessellation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)