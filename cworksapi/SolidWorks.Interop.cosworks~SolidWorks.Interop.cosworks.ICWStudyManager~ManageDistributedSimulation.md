<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~ManageDistributedSimulation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ManageDistributedSimulation Method (ICWStudyManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html) : ManageDistributedSimulation Method (ICWStudyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BOffLoad*
:   True to offload the coordinating computer's simulation processing to other computers on the network, false to let the coordinating computer participate in network simulation

*ComputerNames*
:   Array of names of computers participating in network simulation

Obsolete. Superseded by [ICWStudyManager::ManageDistributedSimulation2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~ManageDistributedSimulation2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ManageDistributedSimulation( _    ByVal BOffLoad As System.Integer, _    ByVal ComputerNames As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyManager Dim BOffLoad As System.Integer Dim ComputerNames As System.Object Dim value As System.Integer   value = instance.ManageDistributedSimulation(BOffLoad, ComputerNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ManageDistributedSimulation(     System.int BOffLoad,    System.object ComputerNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ManageDistributedSimulation(  &   System.int BOffLoad, &   System.Object^ ComputerNames ) ``` | |

#### Parameters

*BOffLoad*
:   True to offload the coordinating computer's simulation processing to other computers on the network, false to let the coordinating computer participate in network simulation

*ComputerNames*
:   Array of names of computers participating in network simulation

#### Return Value

Error code as defined in [swsDistributedSimulationError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsDistributedSimulationError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyManager::ManageDistributedSimulation.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for SOLIDWORKS Simulation Professional or Premium.

Network simulation requires the Intel Direct Sparse solver. Before running network simulation:

1. Set the solver type to [swsSolverType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsSolverType_e.html).swsSolverTypeINTELCluster using one of:
   * [ICWBucklingStudyOptions::SolverType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBucklingStudyOptions~SolverType.html)* [ICWDynamicStudyOptions::SolverType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SolverType.html)* [ICWFrequencyStudyOptions::SolverType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions~SolverType.html)* [ICWNonLinearStudyOptions::SolverType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~SolverType.html)* [ICWStaticStudyOptions::SolverType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~SolverType.html)* [ICWThermalStudyOptions::SolverType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWThermalStudyOptions~SolverType.html)- Call [ICWStudyManager::SetDistributedSimulation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~SetDistributedSimulation.html) to enable network simulation.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html)

[ICWStudyManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager_members.html)

[ICWStudy::GetClusterComputers Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~GetClusterComputers.html)

[ICWStudy::SetClusterComputers Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~SetClusterComputers.html)

[ICWStudy::IsSimulationDistributable Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~IsSimulationDistributable.html)

[ICWStudy::OffLoad Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~OffLoad.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0