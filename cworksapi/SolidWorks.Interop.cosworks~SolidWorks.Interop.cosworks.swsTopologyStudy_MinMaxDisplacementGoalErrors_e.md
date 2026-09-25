<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_MinMaxDisplacementGoalErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsTopologyStudy\_MinMaxDisplacementGoalErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsTopologyStudy\_MinMaxDisplacementGoalErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Topology study minimize maximum displacement goal result codes

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsTopologyStudy_MinMaxDisplacementGoalErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsTopologyStudy_MinMaxDisplacementGoalErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsTopologyStudy_MinMaxDisplacementGoalErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsTopologyStudy_MinMaxDisplacementGoalErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsTopoDGErrCode\_CoordinateSysInvalidOption** | 4 |
| **swsTopoDGErrCode\_CoordinateSysInvalidSelection** | 5 |
| **swsTopoDGErrCode\_CoordinateSysNAError** | 3 = SetCoordinateSystem is available only when SetCoordinateSystemPreference sets NCSPreference = [swsTopologyStudyDisplacementCoordinateSysOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyDisplacementCoordinateSysOption_e.html).swsTopologyDisplacementCoordinateSysOption\_UserDefine |
| **swsTopoDGErrCode\_CoordinateSysNotSelected** | 6 |
| **swsTopoDGErrCode\_InvalidArray** | 8 |
| **swsTopoDGErrCode\_InvalidComponent** | 2 |
| **swsTopoDGErrCode\_InvalidEntities** | 9 |
| **swsTopoDGErrCode\_InvalidVertexCount** | 7 = You must specify at least one vertex for this goal |
| **swsTopoDGErrCode\_SetOperationNotSupported** | 1 = BeginEdit must be called before setting values |
| **swsTopoDGErrCode\_Success** | 0 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)