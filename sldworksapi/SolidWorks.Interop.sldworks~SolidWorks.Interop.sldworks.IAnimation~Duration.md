<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnimation~Duration.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Duration Property (IAnimation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAnimation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnimation.html) : Duration Property (IAnimation) |

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
| ``` ReadOnly Property Duration As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAnimation Dim value As System.Double   value = instance.Duration ``` | |

| C# |  |
| --- | --- |
| ``` System.double Duration {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double Duration {    System.double get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Length of time, in seconds, this animation plays

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Animation::Duration.

# ![](dotnetimages/collapse.gif)Remarks

[IAnimation::Speed](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnimation~Speed.html) affects the duration of the animation. Animation::Speed allows you
to specify whether or not to play the animation at half speed or double speed, which
halves or doubles the animation duration.

If you use Animation::Duration while an animation is playing, then you might not get
the same result as when the animation is not running.

|  |  |  |
| --- | --- | --- |
| **If you get the Animation object using...** | **And then use...** | **Then the duration...** |
| [ISimulation::Animation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISimulation~Animation.html) | Animation::Duration | Is at the normal playing speed |
| [ISimulation::PlayAnimation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISimulation~PlayAnimation.html) | Animation::Duration | Might be a different value because the animation is playing and the **Animation Controller** speed may be set to **Normal**, **Slow Play**, or **Fast Play** |

# ![](dotnetimages/collapse.gif)See Also

####

[IAnimation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnimation.html)

[IAnimation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnimation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14