<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRigidConnectorEndEditError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsRigidConnectorEndEditError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsRigidConnectorEndEditError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Rigid connector editing errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsRigidConnectorEndEditError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsRigidConnectorEndEditError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsRigidConnectorEndEditError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsRigidConnectorEndEditError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsRigidConnectorEndEditErrorBodyExcludedFromAnalysis** | 9 = Selected entity is on a body excluded from analysis |
| **swsRigidConnectorEndEditErrorEntityAlreadyAdded** | 2 = Entity already added |
| **swsRigidConnectorEndEditErrorFacesOnSameComponent** | 8 = Faces are on the same component |
| **swsRigidConnectorEndEditErrorHasBeamBody** | 6 = Connector has a beam body |
| **swsRigidConnectorEndEditErrorHasMassBody** | 7 = Connector has a mass body |
| **swsRigidConnectorEndEditErrorIndexTooBig** | 5 = Specified index > total number of entities |
| **swsRigidConnectorEndEditErrorNoEntityAtIndex** | 1 = No entity at the specified index |
| **swsRigidConnectorEndEditErrorNullEntity** | 10 = Entity is NULL |
| **swsRigidConnectorEndEditErrorSelectFace** | 4 = Select a face |
| **swsRigidConnectorEndEditErrorSelectTargetEntityOrFaces** | 3 = Either the target entity or the faces has not been selected |
| **swsRigidConnectorEndEditErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)