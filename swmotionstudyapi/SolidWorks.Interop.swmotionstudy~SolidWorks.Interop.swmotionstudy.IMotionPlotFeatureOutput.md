<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionPlotFeatureOutput.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| IMotionPlotFeatureOutput Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionPlotFeatureOutput_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) : IMotionPlotFeatureOutput Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a plot's values.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IMotionPlotFeatureOutput ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMotionPlotFeatureOutput ``` | |

| C# |  |
| --- | --- |
| ``` public interface IMotionPlotFeatureOutput ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IMotionPlotFeatureOutput ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MotionPlotFeatureOutput.

# ![](dotnetimages/collapse.gif)Example

[Create Plots and Get Values (C#)](Create_Plots_and_Get_Values_Example_CSharp.htm)

[Create Plots and Get Values (VB.NET)](Create_Plots_and_Get_Values_Example_VBNET.htm)

[Create Plots and Get Values (VBA)](Create_Plots_and_Get_Values_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Typical steps for creating a motion study's plot data and plot:

1. Open an assembly model and create the motion study.- Select the model's entities whose motion you want to measure.- Perform the calculations and get the results.- Create a plot feature data.- Create the plot's x-axis and y-axis feature data objects.- Set the type of plot.- Select the result component.- Set the entities for the x-axis and y-axis feature data objects.- Get the plot's x-axis and y-axis values and insert and display the plot.

Examine the examples to see the calls for these steps.

# ![](dotnetimages/collapse.gif)Accessors

[ICosmosMotionStudyResults::GetValues](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.ICosmosMotionStudyResults~GetValues.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IMotionPlotFeatureOutput Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionPlotFeatureOutput_members.html)

[SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html)