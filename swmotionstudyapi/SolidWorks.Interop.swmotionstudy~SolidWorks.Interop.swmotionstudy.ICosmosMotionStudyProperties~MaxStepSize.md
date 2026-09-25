<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyProperties~MaxStepSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| MaxStepSize Property (ICosmosMotionStudyProperties) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) > [ICosmosMotionStudyProperties Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyProperties.html) : MaxStepSize Property (ICosmosMotionStudyProperties) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the upper bound of the integration time step.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property MaxStepSize As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICosmosMotionStudyProperties Dim value As System.Double   instance.MaxStepSize = value   value = instance.MaxStepSize ``` | |

| C# |  |
| --- | --- |
| ``` System.double MaxStepSize {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double MaxStepSize {    System.double get();    void set ( &   System.double value); } ``` | |

#### Property Value

Upper bound of the integration time step

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CosmosMotionStudyProperties::MaxStepSize.

# ![](dotnetimages/collapse.gif)Remarks

This property is only important if the solver is missing short-lived events, such as impacts. It should be set to the same order as the short-lived events. Integration time can be much longer because the solver cannot move forward as fast.

# ![](dotnetimages/collapse.gif)See Also

####

[ICosmosMotionStudyProperties Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyProperties.html)

[ICosmosMotionStudyProperties Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyProperties_members.html)

[ICosmosMotionStudyProperties::MinStepSize Property](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyProperties~MinStepSize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0