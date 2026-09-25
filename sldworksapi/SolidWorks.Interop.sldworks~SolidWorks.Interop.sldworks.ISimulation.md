<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISimulation Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISimulation Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

This interface is:

* obsolete and has not been superseded.

  * nonfunctional in SOLIDWORKS 2008 and later.

Use the interfaces related to motion studies introduced in SOLIDWORKS 2008 to access animation and simulation.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ISimulation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISimulation ``` | |

| C# |  |
| --- | --- |
| ``` public interface ISimulation ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ISimulation ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Simulation.

# ![](dotnetimages/collapse.gif)Remarks

Do not confuse Physical Simulation with [animation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnimation.html). The SOLIDWORKS software computes a Physical Simulation, which generates a number of steps (and transforms) and elapsed time for those steps. The SOLIDWORKS software then displays the computed Physical Simulation using animation. To create the display, the animation process takes the Physical Simulation steps and does a linear interpolation of those steps for the elapsed time. The elapsed time and frames of Physical Simulation will most likely be different than the elapsed time and frames of an animation.

# ![](dotnetimages/collapse.gif)See Also

####

[ISimulation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)