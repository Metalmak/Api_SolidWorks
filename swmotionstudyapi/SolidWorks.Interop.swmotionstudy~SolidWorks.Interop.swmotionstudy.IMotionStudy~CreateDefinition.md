<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~CreateDefinition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| CreateDefinition Method (IMotionStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) > [IMotionStudy Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy.html) : CreateDefinition Method (IMotionStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   Type of simulation feature as defined in swFeatureNameID\_e:

    * swFmAEMGravity (ISimulationGravityFeatureData)* swFmAEMLinearForce (ISimulationForceFeatureData)* swFmAEMTorque (ISimulationForceFeatureData)* swFmAEMLinearMotor (ISimulationMotorFeatureData)* swFmAEMRotationalMotor (ISimulationMotorFeatureData)* swFmAEMLinearDamper (ISimulationDamperFeatureData)* swFmAEMTorsionalDamper (ISimulationDamperFeatureData)* swFmAEM3DContact (ISimulation3DContactFeatureData)* swFmAEMLinearMotionSpring (ISimulationSpringFeatureData)* swFmAEMTorsionalMotionSpring (ISimulationSpringFeatureData)* swFmAEMLinearSpring (ISimulationLinearSpringFeatureData)

Creates the definition for the simulation feature data object.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateDefinition( _    ByVal Type As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMotionStudy Dim Type As System.Integer Dim value As System.Object   value = instance.CreateDefinition(Type) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateDefinition(     System.int Type ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateDefinition(  &   System.int Type ) ``` | |

#### Parameters

*Type*
:   Type of simulation feature as defined in swFeatureNameID\_e:

    * swFmAEMGravity (ISimulationGravityFeatureData)* swFmAEMLinearForce (ISimulationForceFeatureData)* swFmAEMTorque (ISimulationForceFeatureData)* swFmAEMLinearMotor (ISimulationMotorFeatureData)* swFmAEMRotationalMotor (ISimulationMotorFeatureData)* swFmAEMLinearDamper (ISimulationDamperFeatureData)* swFmAEMTorsionalDamper (ISimulationDamperFeatureData)* swFmAEM3DContact (ISimulation3DContactFeatureData)* swFmAEMLinearMotionSpring (ISimulationSpringFeatureData)* swFmAEMTorsionalMotionSpring (ISimulationSpringFeatureData)* swFmAEMLinearSpring (ISimulationLinearSpringFeatureData)

#### Return Value

Feature data object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MotionStudy::CreateDefinition.

# ![](dotnetimages/collapse.gif)Example

[Add Spring to Motion Study (C#)](Add_Spring_to_Motion_Study_Example_CSharp.htm)

[Add Spring to Motion Study (VB.NET)](Add_Spring_to_Motion_Study_Example_VBNET.htm)

[Add Spring to Motion Study (VBA)](Add_Spring_to_Motion_Study_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can use this method to define a simulation feature data object that is used by [IMotionStudy::CreateFeature](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~CreateFeature.html) to create these simulation features:

* 3DContact* Damper* Force* Gravity* Motor* Spring

A motion study must be active when defining and creating a simulation feature. If a motion study is not active, then this method returns null or Nothing.

# ![](dotnetimages/collapse.gif)See Also

####

[IMotionStudy Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy.html)

[IMotionStudy Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0