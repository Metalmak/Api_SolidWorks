<!-- source: obsoleteapi/EdgeFlangeFeatureData/EdgeFlangeFeatureData__Edge.htm -->

# EdgeFlangeFeatureData::Edge

This property is obsolete and has been superseded
by [EdgeFlangeFeatureData::Edges](..%5CEdge%5CsldworksAPI.chm%3A%3A%5CEdgeFlangeFeatureData%5CEdgeFlangeFeatureData__Edges.htm),
[EdgeFlangeFeatureData::IGetEdges](..%5CEdge%5CsldworksAPI.chm%3A%3A%5CEdgeFlangeFeatureData%5CEdgeFlangeFeatureData__IGetEdges.htm),
and [EdgeFlangeFeatureData::ISetEdges](..%5CEdge%5CsldworksAPI.chm%3A%3A%5CEdgeFlangeFeatureData%5CEdgeFlangeFeatureData__ISetEdges.htm).

Description

This property gets or sets the edge for this
edge flange feature.

Syntax (OLE Automation)

edge = EdgeFlangeFeatureData.Edge (VB Get property)

EdgeFlangeFeatureData.Edge = edge (VB Set property)

edge = EdgeFlangeFeatureData.GetEdge ( ) (C++ Get
property)

EdgeFlangeFeatureData.SetEdge ( edge ) (C++ Set property)

#

| Property: | (LPDISPATCH) edge | Dispatch pointer to the edge |

Syntax (COM)

status = EdgeFlangeFeatureData->get\_Edge ( &edge
)

status = EdgeFlangeFeatureData->put\_Edge ( edge
)

| Property: | (LPDISPATCH) edge | Pointer to the edge |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

See Accessing Selections that
Define Features for details on using this property.