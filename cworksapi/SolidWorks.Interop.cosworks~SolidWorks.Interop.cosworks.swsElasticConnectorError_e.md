<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsElasticConnectorError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsElasticConnectorError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsElasticConnectorError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Elastic connector errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsElasticConnectorError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsElasticConnectorError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsElasticConnectorError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsElasticConnectorError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsElasticConnectorErrorBodyExcludedFromAnalysis** | 10 = Selected entity is on a body excluded from analysis |
| **swsElasticConnectorErrorFaceHasRemoteMassOrBeamBody** | 9 = Selected face has a remote mass or has a beam body |
| **swsElasticConnectorErrorInvalidArray** | 4 = Invalid array |
| **swsElasticConnectorErrorInvalidMesh** | 1 = Invalid mesh |
| **swsElasticConnectorErrorInvalidStudy** | 3 = Invalid study type |
| **swsElasticConnectorErrorNoEntityNoObject** | 7 = No entity selected and object is empty |
| **swsElasticConnectorErrorNonlinearStudyAndPartDocument** | 2 = Study type equals nonlinear and document type equals part |
| **swsElasticConnectorErrorNullOrEmptyArray** | 8 = Array is null or empty |
| **swsElasticConnectorErrorSelectFace** | 5 = Select a face |
| **swsElasticConnectorErrorSelectPlanarFace** | 6 = Select a planar face |
| **swsElasticConnectorErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)Remarks

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)