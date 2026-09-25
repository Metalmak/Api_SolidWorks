<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsTopologyStudyError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsTopologyStudyError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Topology study result codes

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsTopologyStudyError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsTopologyStudyError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsTopologyStudyError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsTopologyStudyError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsTopoErrCode\_CannotCreatFOSIfStressAlrdyPrsnt** | 18 = Factor of Safety constraint cannot be created if a stress constraint is present |
| **swsTopoErrCode\_CannotCreatStressIfFOSAlrdyPrsnt** | 19 = Stress constraint cannot be created if a Factor of Safety constraint is present |
| **swsTopoErrCode\_ConstraintDefinitionLimitReached** | 11 = No more than seven constraints can be defined |
| **swsTopoErrCode\_ConstraintNotFound** | 9 |
| **swsTopoErrCode\_DefaultConstraintCannotBeRemoved** | 10 |
| **swsTopoErrCode\_InvalidGoalType** | 2 |
| **swsTopoErrCode\_ManufacturingControlNotFound** | 12 |
| **swsTopoErrCode\_MaximizeStiffnessGoalHasNotBeenSet** | 5 |
| **swsTopoErrCode\_MinimizeMassGoalHasNotBeenSet** | 4 |
| **swsTopoErrCode\_MinimizeMaximumDisplacementGoalHasNotBeenSet** | 6 |
| **swsTopoErrCode\_NoGoalHasBeenSet** | 3 |
| **swsTopoErrCode\_OnlyOneDemoldControlCanBeDefined** | 14 |
| **swsTopoErrCode\_OnlyOneDisplacementConstraintWithAutoDefineCanBeDefined** | 8 |
| **swsTopoErrCode\_OnlyOneFOSConstraintCanBeDefined** | 21 |
| **swsTopoErrCode\_OnlyOneFrequencyConstraintCanBeDefined** | 16 |
| **swsTopoErrCode\_OnlyOneMassConstraintCanBeDefined** | 7 |
| **swsTopoErrCode\_OnlyOneStressConstraintCanBeDefined** | 20 |
| **swsTopoErrCode\_OnlyOneSymmetryControlCanBeDefined** | 15 |
| **swsTopoErrCode\_OnlyOneThicknessControlCanBeDefined** | 13 |
| **swsTopoErrCode\_SetOperationNotSupported** | 17 = BeginEdit must be called before setting any values |
| **swsTopoErrCode\_Success** | 0 |
| **swsTopoErrCode\_TopologyStudyManagerIsNotInitialized** | 1 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)