<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_PreservedRegionErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsTopologyStudy\_PreservedRegionErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsTopologyStudy\_PreservedRegionErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Topology study preserved region manufacturing control result codes

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsTopologyStudy_PreservedRegionErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsTopologyStudy_PreservedRegionErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsTopologyStudy_PreservedRegionErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsTopologyStudy_PreservedRegionErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsTopoPRErrCode\_InvalidAreaDepth** | 3 = Area depth must be > 0 |
| **swsTopoPRErrCode\_InvalidAreaDepthUnit** | 4 |
| **swsTopoPRErrCode\_InvalidArray** | 5 |
| **swsTopoPRErrCode\_InvalidEntities** | 6 = Input array contains non-face entities |
| **swsTopoPRErrCode\_InvalidFaceCount** | 2 = You must select at least one face |
| **swsTopoPRErrCode\_SetOperationNotSupported** | 1 = BeginEdit must be called before setting values |
| **swsTopoPRErrCode\_Success** | 0 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)