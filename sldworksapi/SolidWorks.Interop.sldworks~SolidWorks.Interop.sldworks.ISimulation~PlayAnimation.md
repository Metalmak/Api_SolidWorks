<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation~PlayAnimation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PlayAnimation Method (ISimulation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISimulation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation.html) : PlayAnimation Method (ISimulation) |

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
| ``` Function PlayAnimation() As Animation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISimulation Dim value As Animation   value = instance.PlayAnimation() ``` | |

| C# |  |
| --- | --- |
| ``` Animation PlayAnimation() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Animation^ PlayAnimation(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

[Animation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnimation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Simulation::PlayAnimation.

# ![](dotnetimages/collapse.gif)Remarks

If an animation is playing when this method is used, then this method returns the [IAnimation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnimation.html) object for that animation. To check to see if an animation is currently playing, use [ISimulation::IsAnimationPlaying](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISimulation~IsAnimationPlaying.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISimulation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation.html)

[ISimulation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0