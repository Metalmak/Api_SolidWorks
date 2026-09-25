<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IPhysicalSimulationMotionStudyProperties~MateAccuracy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| MateAccuracy Property (IPhysicalSimulationMotionStudyProperties) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) > [IPhysicalSimulationMotionStudyProperties Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IPhysicalSimulationMotionStudyProperties.html) : MateAccuracy Property (IPhysicalSimulationMotionStudyProperties) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the mate accuracy for this Physical Simulation motion study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property MateAccuracy As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPhysicalSimulationMotionStudyProperties Dim value As System.Integer   instance.MateAccuracy = value   value = instance.MateAccuracy ``` | |

| C# |  |
| --- | --- |
| ``` System.int MateAccuracy {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int MateAccuracy {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Mate accuracy

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PhysicalSimulationMotionStudyProperties::MateAccuracy.

# ![](dotnetimages/collapse.gif)Remarks

This property controls the amount of interpenetration of geometric meshes. A lower value for Accuracy allows more mesh interpenetration. This allows for smother motion, especially in tight-fit situations; for example, a ball rolling in a channel with very little clearance.

# ![](dotnetimages/collapse.gif)See Also

####

[IPhysicalSimulationMotionStudyProperties Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IPhysicalSimulationMotionStudyProperties.html)

[IPhysicalSimulationMotionStudyProperties Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IPhysicalSimulationMotionStudyProperties_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0