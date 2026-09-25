<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~BondingFormulation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| BondingFormulation Property (ICWContactComponent) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWContactComponent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent.html) : BondingFormulation Property (ICWContactComponent) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Sets the bonding formulation for this contact.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` WriteOnly Property BondingFormulation As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWContactComponent   instance.BondingFormulation = value ``` | |

| C# |  |
| --- | --- |
| ``` System.int BondingFormulation {set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int BondingFormulation {    void set ( &   System.int value); } ``` | |

#### Property Value

Option for

* no penetration ([static](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWStaticStudyOptions.html) and [nonlinear](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWNonLinearStudyOptions.html) studies only) advanced options as defined in [swsNoPenetrationOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNoPenetrationOption_e.html) (except swsNoPenetrationOptionNodeToNode)* thermal resistance ([thermal](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWThermalStudyOptions.html) studies only) advanced options as defined in [swsNoPenetrationOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNoPenetrationOption_e.html) (except swsNoPenetrationOptionNodeToNode)* shrink fit (static and nonlinear studies only) advanced options as defined in [swsShrinkFitOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsShrinkFitOption_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWContactComponent::BondingFormulation.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only for selected components that behave during simulation as if they were welded.

For more information, see **SOLIDWORKS user-interface Help > Simulation > Interaction Options >**:

* **Component Interaction PropertyManager**

     - and -

* **Types of Interactions > Bonded Interaction**

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactComponent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent.html)

[ICWContactComponent Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2022 SP1