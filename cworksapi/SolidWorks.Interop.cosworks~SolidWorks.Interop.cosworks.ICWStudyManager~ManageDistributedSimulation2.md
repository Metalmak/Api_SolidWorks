<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~ManageDistributedSimulation2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ManageDistributedSimulation2 Method (ICWStudyManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html) : ManageDistributedSimulation2 Method (ICWStudyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BOffLoad*
:   -1 or true to offload the coordinating computer's simulation processing to other computers on the network, 0 or false to let the coordinating computer participate in network simulation

*ComputerNames*
:   Array of names of computers participating in network simulation

Sets up network simulation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ManageDistributedSimulation2( _    ByVal BOffLoad As System.Boolean, _    ByVal ComputerNames As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyManager Dim BOffLoad As System.Boolean Dim ComputerNames As System.Object Dim value As System.Integer   value = instance.ManageDistributedSimulation2(BOffLoad, ComputerNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ManageDistributedSimulation2(     System.bool BOffLoad,    System.object ComputerNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ManageDistributedSimulation2(  &   System.bool BOffLoad, &   System.Object^ ComputerNames ) ``` | |

#### Parameters

*BOffLoad*
:   -1 or true to offload the coordinating computer's simulation processing to other computers on the network, 0 or false to let the coordinating computer participate in network simulation

*ComputerNames*
:   Array of names of computers participating in network simulation

#### Return Value

Error code as defined in [swsDistributedSimulationError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsDistributedSimulationError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyManager::ManageDistributedSimulation2.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html)

[ICWStudyManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2022 SP0