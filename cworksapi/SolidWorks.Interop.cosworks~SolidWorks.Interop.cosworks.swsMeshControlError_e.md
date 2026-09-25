<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshControlError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsMeshControlError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsMeshControlError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Mesh control errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsMeshControlError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsMeshControlError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsMeshControlError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsMeshControlError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsMeshControlErrorElementSize** | 6 = Specify a number between 0.0000001 and 1000000 for element size |
| **swsMeshControlErrorEntityAlreadyExists** | 2 = Entity already exists in this mesh control |
| **swsMeshControlErrorNoEntities** | 3 = No entities selected |
| **swsMeshControlErrorNoEntityAtIndex** | 1 = No entity is passed at index |
| **swsMeshControlErrorNumberOfLayers** | 7 = Number of layers must be an integer larger than 0 and less than or equal to 80 |
| **swsMeshControlErrorSelectFaceEdgeOrVertex** | 5 = Select face, edge, or vertex |
| **swsMeshControlErrorSelectVerticesEdgesFacesBodiesOrComponents** | 4 = Select vertices, edges, faces, bodies, or components |
| **swsMeshControlErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)