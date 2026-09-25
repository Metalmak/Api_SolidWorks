<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IPhysicalSimulationMotionStudyProperties~GeometricAccuracy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| GeometricAccuracy Property (IPhysicalSimulationMotionStudyProperties) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) > [IPhysicalSimulationMotionStudyProperties Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IPhysicalSimulationMotionStudyProperties.html) : GeometricAccuracy Property (IPhysicalSimulationMotionStudyProperties) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the geometric accuracy of this Physical Simulation motion study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property GeometricAccuracy As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPhysicalSimulationMotionStudyProperties Dim value As System.Integer   instance.GeometricAccuracy = value   value = instance.GeometricAccuracy ``` | |

| C# |  |
| --- | --- |
| ``` System.int GeometricAccuracy {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int GeometricAccuracy {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

 Geometric accuracy

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PhysicalSimulationMotionStudyProperties::GeometricAccuracy.

# ![](dotnetimages/collapse.gif)Remarks

Physical Simulation creates meshes from curved geometry. The higher the value for Accuracy, the closer to actual geometry the mesh becomes. This makes collision simulation more accurate, but requires more time to compute.

# ![](dotnetimages/collapse.gif)See Also

####

[IPhysicalSimulationMotionStudyProperties Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IPhysicalSimulationMotionStudyProperties.html)

[IPhysicalSimulationMotionStudyProperties Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IPhysicalSimulationMotionStudyProperties_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0