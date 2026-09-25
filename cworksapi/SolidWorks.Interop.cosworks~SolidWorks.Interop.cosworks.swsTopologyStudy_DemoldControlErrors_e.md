<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_DemoldControlErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsTopologyStudy\_DemoldControlErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsTopologyStudy\_DemoldControlErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Topology study de-mold manufacturing control result codes

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsTopologyStudy_DemoldControlErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsTopologyStudy_DemoldControlErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsTopologyStudy_DemoldControlErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsTopologyStudy_DemoldControlErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsTopoDCErrCode\_EdgeSelectionNotAvailable** | 8 = Edge selection is not available for [swsTopologyStudyDemoldDirectionOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyDemoldDirectionOption_e.html).swsTopologyDemoldDirection\_TwoDirectionMidPlane de-mold direction option when SetAutoDetermineCentralMidPlane sets BFlag = 0 |
| **swsTopoDCErrCode\_EdgeSelectionRequired** | 9 = Edge selection is required for all de-mold direction options except swsTopologyStudyDemoldDirectionOption\_e.swsTopologyDemoldDirection\_TwoDirectionMidPlane when SetAutoDetermineCentralMidPlane sets BFlag = 0 |
| **swsTopoDCErrCode\_InvalidDirectionOptionSelected** | 3 |
| **swsTopoDCErrCode\_InvalidEntitySelectedAsEdge** | 2 |
| **swsTopoDCErrCode\_InvalidEntitySelectedAsPlane** | 4 |
| **swsTopoDCErrCode\_NotAvailableForCurrentDirectionOption** | 5 |
| **swsTopoDCErrCode\_PlaneSelectionNotAvailable** | 6 = Plane selection is available only for swsTopologyStudyDemoldDirectionOption\_e.swsTopologyDemoldDirection\_TwoDirectionMidPlane de-mold direction option when SetAutoDetermineCentralMidPlane sets BFlag = 0 |
| **swsTopoDCErrCode\_PlaneSelectionRequired** | 7 = Plane selection is required for swsTopologyStudyDemoldDirectionOption\_e.swsTopologyDemoldDirection\_TwoDirectionMidPlane de-mold direction option when SetAutoDetermineCentralMidPlane sets BFlag = 0 |
| **swsTopoDCErrCode\_SetOperationNotSupported** | 1 = BeginEdit must be called before setting values |
| **swsTopoDCErrCode\_Success** | 0 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)