<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~SetClusterComputers.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetClusterComputers Method (ICWStudy) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html) : SetClusterComputers Method (ICWStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ComputerNames*
:   Array of computer names

Sets the list of names of the computers participating in this study's distributed simulation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetClusterComputers( _    ByVal ComputerNames As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudy Dim ComputerNames As System.Object Dim value As System.Integer   value = instance.SetClusterComputers(ComputerNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetClusterComputers(     System.object ComputerNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetClusterComputers(  &   System.Object^ ComputerNames ) ``` | |

#### Parameters

*ComputerNames*
:   Array of computer names

#### Return Value

Error code as defined in [swsDistributedSimulationError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsDistributedSimulationError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudy::SetClusterComputers.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if:

* The license is SOLIDWORKS Simulation Professional or Premium.* [ICWStudy::IsSimulationDistributable](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~IsSimulationDistributable.html) is true.* [ICWStudy::OffLoad](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~OffLoad.html) is true.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudy Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy_members.html)

[ICWStudy::GetClusterComputers Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~GetClusterComputers.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0