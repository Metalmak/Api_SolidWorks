<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IEdge Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IEdge Interface |

The following tables list the members exposed by [IEdge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Check](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~Check.html) | Gets whether the edge is a valid, and, if not, returns the faults. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [CreateWireBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~CreateWireBody.html) | Creates a wire body from this edge. |
| ![ Method](dotnetimages/Method.gif) | [Display](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~Display.html) | Highlights this edge with the specified color. |
| ![ Method](dotnetimages/Method.gif) | [EdgeInFaceSense](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~EdgeInFaceSense.html) | Checks whether the edge and the loop lying on the specified face have the same direction (sense). |
| ![ Method](dotnetimages/Method.gif) | [EnumCoEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~EnumCoEdges.html) | Lists the coedges that reference this edge. |
| ![ Method](dotnetimages/Method.gif) | [Evaluate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~Evaluate.html) | Obsolete. Superseded by [IEdge::Evaluate2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~Evaluate2.html). |
| ![ Method](dotnetimages/Method.gif) | [Evaluate2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~Evaluate2.html) | Evaluates the edge for the specified U parameter. |
| ![ Method](dotnetimages/Method.gif) | [GetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetBody.html) | Gets the body for this edge. |
| ![ Method](dotnetimages/Method.gif) | [GetClosestPointOn](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetClosestPointOn.html) | Uses the X,Y,Z input point and returns the closest point on the edge. |
| ![ Method](dotnetimages/Method.gif) | [GetCoEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetCoEdges.html) | Gets the coedges that reference this edge. |
| ![ Method](dotnetimages/Method.gif) | [GetCurve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetCurve.html) | Gets the underlying curve for this edge. |
| ![ Method](dotnetimages/Method.gif) | [GetCurveParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetCurveParams.html) | Obsolete. Superseded by [IEdge::GetCurveParams2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~GetCurveParams2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetCurveParams2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetCurveParams2.html) | Obsolete. Superseded by [IEdge::GetCurveParams3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~GetCurveParams3.html). |
| ![ Method](dotnetimages/Method.gif) | [GetCurveParams3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetCurveParams3.html) | Gets a data object containing the curve parameters for this edge. |
| ![ Method](dotnetimages/Method.gif) | [GetEndVertex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetEndVertex.html) | Gets the ending vertex for this edge. |
| ![ Method](dotnetimages/Method.gif) | [GetID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetID.html) | Gets the edge ID of this edge in an imported body. |
| ![ Method](dotnetimages/Method.gif) | [GetParameter](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetParameter.html) | Gets the parameterization of the edge. |
| ![ Method](dotnetimages/Method.gif) | [GetStartVertex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetStartVertex.html) | Gets the starting vertex for this edge. |
| ![ Method](dotnetimages/Method.gif) | [GetTangentEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetTangentEdges.html) | Gets all of the edges tangent to this edge. |
| ![ Method](dotnetimages/Method.gif) | [GetTangentEdgesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetTangentEdgesCount.html) | Gets the number of edges tangent to this edge. |
| ![ Method](dotnetimages/Method.gif) | [GetTrackingIDs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetTrackingIDs.html) | Gets the [tracking IDs assigned to this edge](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~SetTrackingID.html). |
| ![ Method](dotnetimages/Method.gif) | [GetTrackingIDsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetTrackingIDsCount.html) | Gets the number of tracking IDs on this edge. |
| ![ Method](dotnetimages/Method.gif) | [GetTwoAdjacentFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetTwoAdjacentFaces.html) | Obsolete. Superseded by [IEdge::GetTwoAdjacentFaces2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~GetTwoAdjacentFaces2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetTwoAdjacentFaces2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~GetTwoAdjacentFaces2.html) | Gets the two faces adjacent to an edge. |
| ![ Method](dotnetimages/Method.gif) | [Highlight](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~Highlight.html) | Add highlights or removes highlights from this edge. |
| ![ Method](dotnetimages/Method.gif) | [IEdgeInFaceSense](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IEdgeInFaceSense.html) | Obsolete. Superseded by [IEdge::IEdgeInFaceSense2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~IEdgeInFaceSense2.html). |
| ![ Method](dotnetimages/Method.gif) | [IEdgeInFaceSense2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IEdgeInFaceSense2.html) | Checks whether the edge and the loop lying on the specified face have the same direction (sense). |
| ![ Method](dotnetimages/Method.gif) | [IEvaluate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IEvaluate.html) | Obsolete. Superseded by [IEdge::IEvaluate2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~IEvaluate2.html). |
| ![ Method](dotnetimages/Method.gif) | [IEvaluate2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IEvaluate2.html) | Evaluates the edge for the specified U parameter. |
| ![ Method](dotnetimages/Method.gif) | [IGetClosestPointOn](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IGetClosestPointOn.html) | Uses the X,Y,Z input point and returns the closest point on the edge. |
| ![ Method](dotnetimages/Method.gif) | [IGetCurve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IGetCurve.html) | Gets the underlying curve for this edge. |
| ![ Method](dotnetimages/Method.gif) | [IGetCurveParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IGetCurveParams.html) | Obsolete. Superseded by [IEdge::IGetCurveParams2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~IGetCurveParams2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetCurveParams2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IGetCurveParams2.html) | Returns the curve parameters for this edge, including the edge and curve direction (sense). |
| ![ Method](dotnetimages/Method.gif) | [IGetEndVertex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IGetEndVertex.html) | Gets the ending vertex for this edge. |
| ![ Method](dotnetimages/Method.gif) | [IGetParameter](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IGetParameter.html) | Gets the parameterization of the edge. |
| ![ Method](dotnetimages/Method.gif) | [IGetStartVertex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IGetStartVertex.html) | Gets the starting vertex for this edge. |
| ![ Method](dotnetimages/Method.gif) | [IGetTangentEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IGetTangentEdges.html) | Gets all of the edges tangent to this edge. |
| ![ Method](dotnetimages/Method.gif) | [IGetTrackingIDs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IGetTrackingIDs.html) | Gets the [tracking IDs assigned to this edge](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~SetTrackingID.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetTwoAdjacentFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IGetTwoAdjacentFaces.html) | Obsolete. Superseded by [IEdge::IGetTwoAdjacentFaces2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~IGetTwoAdjacentFaces2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetTwoAdjacentFaces2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IGetTwoAdjacentFaces2.html) | Gets the two faces adjacent to an edge. |
| ![ Method](dotnetimages/Method.gif) | [IsParamReversed](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IsParamReversed.html) | Gets whether the edge and its underlying curve have the same parameterization or if the direction is reversed. |
| ![ Method](dotnetimages/Method.gif) | [IsTolerant](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IsTolerant.html) | Gets whether an edge is tolerant and its tolerance value. |
| ![ Method](dotnetimages/Method.gif) | [RemoveId](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~RemoveId.html) | Removes the edge ID assigned to this edge of an imported body. |
| ![ Method](dotnetimages/Method.gif) | [RemoveRedundantTopology](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~RemoveRedundantTopology.html) | Removes redundant topology from the edge. |
| ![ Method](dotnetimages/Method.gif) | [RemoveTrackingID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~RemoveTrackingID.html) | Removes a [tracking ID assigned to this edge](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~SetTrackingID.html). |
| ![ Method](dotnetimages/Method.gif) | [SetId](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~SetId.html) | Sets the edge ID of this edge of an imported body. |
| ![ Method](dotnetimages/Method.gif) | [SetTrackingID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~SetTrackingID.html) | Assigns a tracking ID to this edge. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdge Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)