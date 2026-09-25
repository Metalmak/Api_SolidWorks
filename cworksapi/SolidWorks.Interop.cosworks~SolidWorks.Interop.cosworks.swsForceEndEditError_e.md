<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsForceEndEditError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsForceEndEditError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsForceEndEditError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Force editing errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsForceEndEditError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsForceEndEditError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsForceEndEditError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsForceEndEditError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsForceEndEditErrorEntityAlreadyExists** | 2 = Entity already exists in this object |
| **swsForceEndEditErrorMagnitudeForceMustBeLargerZero** | 11 = The magnitude of force must be larger than 0 |
| **swsForceEndEditErrorNoEntitiesSelected** | 3 = No entities selected |
| **swsForceEndEditErrorNoEntityAtIndex** | 1 = No entity passed at index |
| **swsForceEndEditErrorReferenceGeometryEntityNotSelected** | 5 = Entity for reference geometry may not be in the list of selected entities |
| **swsForceEndEditErrorSelectCoordinateSystem** | 8 = Select a coordinate system |
| **swsForceEndEditErrorSelectFace** | 7 = Select only face for entity |
| **swsForceEndEditErrorSelectFaceEdgeOrVertex** | 4 = Select face, edge, or vertex for entity |
| **swsForceEndEditErrorSelectFaceEdgePlaneOrAxisForReferenceGeometry** | 6 = Select face, edge, plane, or axis for reference geometry |
| **swsForceEndEditErrorSelectReferenceAxisOrCylindricalFaceForTorque** | 10 = Select a reference axis or cylindrical face to apply torque |
| **swsForceEndEditErrorSuccessful** | 0 = Successful |
| **swsForceEndEditErrorVariableForceCannotBeAppliedToVertices** | 12 = Variable force cannot be applied to vertices |
| **swsForceEndEditErrorVariableForceCannotBeAppliedToVerticesOrEdges** | 9 = Variable force cannot be applied to vertices or edges |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)