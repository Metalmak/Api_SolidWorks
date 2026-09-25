<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRestraintEndEditError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsRestraintEndEditError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsRestraintEndEditError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Restraint editing errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsRestraintEndEditError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsRestraintEndEditError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsRestraintEndEditError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsRestraintEndEditError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsRestraintEndEditErrorCannotRestrainRefGeometryEntity** | 14 = Entity for reference geometry cannot be in list of entities to be restrained |
| **swsRestraintEndEditErrorCyclicSymmetryRestraint** | 10 = Cyclic symmetry restraint is valid only for solid meshes |
| **swsRestraintEndEditErrorDefineDisplacementComponent** | 13 = Define at least one displacement component |
| **swsRestraintEndEditErrorEntityExists** | 2 = Entity already exists in this restraint |
| **swsRestraintEndEditErrorNoEntity** | 3 = No entity specified |
| **swsRestraintEndEditErrorNoIndex** | 1 = No entity at specified index |
| **swsRestraintEndEditErrorSelectAxis** | 12 = Select axis as reference geometry |
| **swsRestraintEndEditErrorSelectCylindricalFaces** | 6 = Select cylindrical faces |
| **swsRestraintEndEditErrorSelectFaceEdgeOrVertices** | 4 = Select face, edge or vertices |
| **swsRestraintEndEditErrorSelectFaceEdgeVertexOrFaces** | 8 = Select face, edge, vertex, or faces |
| **swsRestraintEndEditErrorSelectFaces** | 5 = Select faces |
| **swsRestraintEndEditErrorSelectPlaneAxisEdgeFaceOrCylinder** | 9 = Select reference plane, axis, edge, planar face, or cylinder for reference |
| **swsRestraintEndEditErrorSelectSphericalFaces** | 7 = Select spherical faces |
| **swsRestraintEndEditErrorSelectTwoFaces** | 11 = Select only two faces for cyclic symmetry |
| **swsRestraintEndEditErrorSuccess** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)