<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation~Animation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Animation Property (ISimulation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISimulation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation.html) : Animation Property (ISimulation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Obsolete. Not superseded.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property Animation As Animation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISimulation Dim value As Animation   value = instance.Animation ``` | |

| C# |  |
| --- | --- |
| ``` Animation Animation {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property Animation^ Animation {    Animation^ get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

[Animation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnimation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Simulation::Animation.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **To...** | **Then..**. |
| Get the duration of an animation | Use [IAnimation::Duration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnimation~Duration.html) after using this property |
| Play the animation | Use [IAnimation::Play](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnimation~Play.html) after using this property |
| Display the Animation Controller pop-up toolbar | Use [ISimulation::PlayAnimation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISimulation~PlayAnimation.html) instead of using this property |

NOTE: Use only the following IAnimation property and method with ISimulation::Animation: IAnimation::Duration and IAnimation::PlayAnimation. The other IAnimation properties and methods do nothing with an IAnimation object returned by ISimlulation::Animation because they expect an animation to be playing. Use [ISimluation::IsAnimationPlaying](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISimulation~IsAnimationPlaying.html) to determine whether an animation is playing.

# ![](dotnetimages/collapse.gif)See Also

####

[ISimulation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation.html)

[ISimulation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0