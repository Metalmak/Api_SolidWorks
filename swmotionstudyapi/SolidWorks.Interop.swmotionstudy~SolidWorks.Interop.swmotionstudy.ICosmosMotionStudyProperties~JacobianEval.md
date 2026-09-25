<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyProperties~JacobianEval.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| JacobianEval Property (ICosmosMotionStudyProperties) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) > [ICosmosMotionStudyProperties Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyProperties.html) : JacobianEval Property (ICosmosMotionStudyProperties) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets how often the simulation engine's Jacobian matrix is updated.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property JacobianEval As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICosmosMotionStudyProperties Dim value As System.Integer   instance.JacobianEval = value   value = instance.JacobianEval ``` | |

| C# |  |
| --- | --- |
| ``` System.int JacobianEval {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int JacobianEval {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

How often, in percent, the simulation engine's Jacobian matrix is updated

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CosmosMotionStudyProperties::JacobianEval.

# ![](dotnetimages/collapse.gif)Remarks

At 100%, the Jacobian is updated at every integration time step. At 50% the Jacobian is updated at every other integration time step. This value impacts models that contain intermittent curve/curve contact. The higher the value, the better the simulation accuracy. However, the higher the value, the greater the impact in the overall simulation time.

# ![](dotnetimages/collapse.gif)See Also

####

[ICosmosMotionStudyProperties Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyProperties.html)

[ICosmosMotionStudyProperties Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyProperties_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0