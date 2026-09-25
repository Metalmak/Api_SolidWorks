<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsBoltConnectorError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsBoltConnectorError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsBoltConnectorError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Bolt connector errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsBoltConnectorError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsBoltConnectorError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsBoltConnectorError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsBoltConnectorError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsBoltConnectorErrorArrayEmpty** | 17 = Array has an empty dispatch |
| **swsBoltConnectorErrorBodyExcludedFromAnalysis** | 20 = Selected entity is on a body excluded from analysis |
| **swsBoltConnectorErrorBoltDiameterTooLarge** | 19 = Bolt diameter may be too large |
| **swsBoltConnectorErrorEdgeFromSameFace** | 21 = Selected edge belongs to a conical face of the same bolt |
| **swsBoltConnectorErrorInvalidMesh** | 1 = Invalid mesh type |
| **swsBoltConnectorErrorInvalidStudy** | 3 = Invalid study |
| **swsBoltConnectorErrorNonLinearStudyAndPartDocument** | 2 = Study type equals nonlinear and document type equals part |
| **swsBoltConnectorErrorNoObjectForNutOrHead** | 15 = No object for either the nut or head |
| **swsBoltConnectorErrorSameEntityHeadAndNut** | 13 = Entity is the same for the head and nut |
| **swsBoltConnectorErrorSelectAssemblyDocument** | 14 = Document type is part; select an assembly document |
| **swsBoltConnectorErrorSelectCircularEdgeOnShells** | 18 = Select circular edge on shells |
| **swsBoltConnectorErrorSelectConcentricEntities** | 9 = Select concentric entities |
| **swsBoltConnectorErrorSelectCylindricalThreadFace** | 8 = Select cylindrical thread face from a different body |
| **swsBoltConnectorErrorSelectDatumPlane** | 10 = Select datum plane |
| **swsBoltConnectorErrorSelectEdge** | 11 = Select an edge |
| **swsBoltConnectorErrorSelectEdgeWithCircularLine** | 6 = Select an edge with circular line |
| **swsBoltConnectorErrorSelectEntity** | 4 = Select an entity |
| **swsBoltConnectorErrorSelectFace** | 12 = Select a face |
| **swsBoltConnectorErrorSelectFaceWithConicalSurface** | 5 = Select a face with conical surface |
| **swsBoltConnectorErrorSelectFaceWithCylindricalSurface** | 7 = Select a face with cylindrical surface |
| **swsBoltConnectorErrorSelectNutOrHead** | 16 = Number of entities selected for the nut or head is < 1 |
| **swsBoltConnectorErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)