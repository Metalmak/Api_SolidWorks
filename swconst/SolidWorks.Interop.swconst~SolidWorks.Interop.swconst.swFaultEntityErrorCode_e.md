<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swFaultEntityErrorCode_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swFaultEntityErrorCode\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swFaultEntityErrorCode\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Fault entity error codes.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swFaultEntityErrorCode_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swFaultEntityErrorCode_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swFaultEntityErrorCode_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swFaultEntityErrorCode_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swBodyCorrupt** | 1 = Data structure is corrupt |
| **swBodyInsideOut** | 3 = Body is inside out |
| **swBodyInvalidIdentifiers** | 2 = Body has invalid or duplicate identifiers |
| **swBodyRegionsInconsistent** | 4 = Regions of body are inconsistent |
| **swEdgeBadFaceOrder** | 14 = On a non-manifold edge, the face order around the edge does not match the order of the faces' surfaces around the edge |
| **swEdgeBadWire** | 15 = Two wireframe edges intersect at a position other than a vertex |
| **swEdgeNonPeriodicCurve** | 5 = Open or non-periodic curve on ring edge |
| **swEdgeNonPeriodicNomGeom** | 6 = Open or non-periodic nominal geometry on ring edge |
| **swEdgeSpcurveOutOfTol** | 11 = Spcurve not within edge's tolerance |
| **swEdgeSpcurveOutOfTolNomGeom** | 12 = Spcurve not within edge's tolerance of nominal geometry |
| **swEdgeTouchEdge** | 36 = Edges touch |
| **swEdgeVertexNotLie** | 7 = Vertex does not lie on edge's curve |
| **swEdgeVertexNotLieNomGeom** | 8 = Vertex does not lie on nominal geometry |
| **swEdgeVerticesTouch** | 13 = Vertices of edge touch |
| **swEdgeWrongDir** | 9 = Curve in wrong direction for edge |
| **swEdgeWrongDirNomGeom** | 10 = Nominal geometry in wrong direction |
| **swEntityStateInvalid** | 34 = State of entity is invalid |
| **swFaceBadEdge** | 17 = Edge does not lie on face's surface |
| **swFaceBadEdgeOrder** | 18 = Edge order around the face does not match the order of the edges' curves around the face |
| **swFaceBadLoops** | 20 = Loops inconsistent |
| **swFaceBadVertex** | 16 = Vertex does not lie on face's surface |
| **swFaceBadWireframe** | 22 = A wireframe edge intersects a face at a position other than a vertex |
| **swFaceCheckerFailure** | 23 = Checker failure during face/face check |
| **swFaceFaceInconsistency** | 24 = Inconsistent faces |
| **swFaceNoAccomVertex** | 19 = A surface singularity has no accompanying vertex |
| **swFaceSelfIntersecting** | 21 = Face is self intersecting |
| **swGeomDegenerate** | 26 = Geometry degenerated |
| **swGeomStateSelfIntersect** | 25 = Geometry is self intersecting |
| **swRegionBadShells** | 27 = Inconsistent shells |
| **swShellBadTopologyGeometry** | 28 = A topological entity belonging to a shell is not geometrically within the shell |
| **swShellIntersect** | 29 = Shell shell inconsistency |
| **swTopolMissingGeometry** | 35 = Missing geometry |
| **swTopolNotG1Continuous** | 30 = Topology's geometry is not G1 continuous |
| **swTopolSizeBoxViolation** | 31 = Some or all of entity is outside size box |
| **swTopolStateCheckFail** | 32 = Checker failure |
| **swTopolStateNoGeometry** | 33 = Missing geometry |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)