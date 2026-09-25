<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinkConnectorError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsLinkConnectorError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsLinkConnectorError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Link connector errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsLinkConnectorError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsLinkConnectorError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsLinkConnectorError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsLinkConnectorError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsLinkConnectorErrorBodyExcludedFromAnalysis** | 8 = Selected entity is on a body excluded from analysis |
| **swsLinkConnectorErrorEmptyEntity** | 5 = Either of the entities is empty |
| **swsLinkConnectorErrorHasRemoteMassOrBeamBody** | 7 = Connect has a remote mass or beam body |
| **swsLinkConnectorErrorInvalidMesh** | 1 = Invalid mesh type |
| **swsLinkConnectorErrorInvalidStudy** | 3 = Invalid study type |
| **swsLinkConnectorErrorNonlinearStudyPartDocument** | 2 = Study type equals nonlinear and document type equals part |
| **swsLinkConnectorErrorSelectAssemblyDocument** | 4 = Select assembly document |
| **swsLinkConnectorErrorSelectVertexOrDatumPoint** | 6 = Select a vertex or datum point |
| **swsLinkConnectorErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)