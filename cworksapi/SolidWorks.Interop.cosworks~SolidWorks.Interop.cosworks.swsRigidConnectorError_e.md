<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRigidConnectorError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsRigidConnectorError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsRigidConnectorError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Rigid connector errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsRigidConnectorError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsRigidConnectorError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsRigidConnectorError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsRigidConnectorError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsRigidConnectorErrorBodyExcludedFromAnalysis** | 14 = Selected entity is on a body excluded from analysis |
| **swsRigidConnectorErrorBodyHasRemoteMass** | 11 = Select body has a remote mass |
| **swsRigidConnectorErrorFacesFromSameComponent** | 13 = Faces are from the same component |
| **swsRigidConnectorErrorInvalidMesh** | 1 = Invalid mesh |
| **swsRigidConnectorErrorInvalidSourceArray** | 5 = Invalid array for the source |
| **swsRigidConnectorErrorInvalidStudy** | 3 = Invalid study type |
| **swsRigidConnectorErrorInvalidTargetArray** | 7 = Invalid array for the target |
| **swsRigidConnectorErrorNonlinearStudyPartDocument** | 2 = Study type equals nonlinear and document type equals part |
| **swsRigidConnectorErrorNoObjectForFace** | 6 = No object for the face |
| **swsRigidConnectorErrorNoObjectForTarget** | 8 = No object for target |
| **swsRigidConnectorErrorNullOrEmptyArray** | 12 = Array of either entities are NULL or empty |
| **swsRigidConnectorErrorSameEntityAtFaceAndTargetArray** | 10 = Entity is the same at face and target array |
| **swsRigidConnectorErrorSelectAssemblyDocument** | 4 = Select assembly document |
| **swsRigidConnectorErrorSelectFace** | 9 = Select a face |
| **swsRigidConnectorErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)