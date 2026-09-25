<!-- source: sldworksapiprogguide/Overview/Tessellation_and_Edges.htm -->

# SOLIDWORKS API Help

# Tessellation and Edges

A couple of approaches are available for finding tessellations for edges.

* Get the range of the curve and tessellate the
  curve along that range.

1. Use IEdge::GetCurve
   to get the curve.
2. Use IEdge::GetCurveParams2
   to determine the range of the curve used by the edge.
3. Use ICurve::GetTessPts
   to tessellate the curve along the range.

  -
or -

* Use IFace2::GetTessTriStripEdges
  to get the indices into the tessellation that represents the edges of
  the face.

The first approach gives you better control over the edge. The second
approach gives you a tight boundary if you are rendering edges and faces
at the same time.