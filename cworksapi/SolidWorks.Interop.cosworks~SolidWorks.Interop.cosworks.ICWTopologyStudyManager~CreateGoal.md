<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager~CreateGoal.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CreateGoal Method (ICWTopologyStudyManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager.html) : CreateGoal Method (ICWTopologyStudyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NGoalType*
:   Type of optimization goal to create as defined in [swsTopologyStudyGoalType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyGoalType_e.html)

Adds the specified optimization goal to this topology study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateGoal( _    ByVal NGoalType As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyStudyManager Dim NGoalType As System.Integer Dim value As System.Integer   value = instance.CreateGoal(NGoalType) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CreateGoal(     System.int NGoalType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CreateGoal(  &   System.int NGoalType ) ``` | |

#### Parameters

*NGoalType*
:   Type of optimization goal to create as defined in [swsTopologyStudyGoalType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyGoalType_e.html)

#### Return Value

Result code as defined in [swsTopologyStudyError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyStudyManager::CreateGoal.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologyStudyManager](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager.html) example.

# ![](dotnetimages/collapse.gif)Remarks

Only one optimization goal can be set in a topology study. A default constraint is automatically created in some cases.

| If the goal is... | Then its default constraint is... |
| --- | --- |
| Maximize stiffness (best stiffness to weight ratio) | Mass ([ICWTopologyMassConstraint](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint.html)) |
| Minimize maximum displacement | Mass (ICWTopologyMassConstraint) |
| Minimize mass with displacement constraint | N/A |

It is not possible to remove the default constraint, either through the user interface or through the API, but it is possible to modify its properties.

You can add up to two different constraints for a given optimization goal.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager.html)

[ICWTopologyStudyManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0