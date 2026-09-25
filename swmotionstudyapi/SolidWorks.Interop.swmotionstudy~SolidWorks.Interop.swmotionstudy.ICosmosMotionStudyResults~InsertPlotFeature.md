<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyResults~InsertPlotFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| InsertPlotFeature Method (ICosmosMotionStudyResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) > [ICosmosMotionStudyResults Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyResults.html) : InsertPlotFeature Method (ICosmosMotionStudyResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PlotFeatureData*
:   Plot's feature data

*PlotXFeatureData*
:   Plot's x-axis feature data

*PlotYFeatureData*
:   Plot's y-axis feature data

Inserts a plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertPlotFeature( _    ByVal PlotFeatureData As System.Object, _    ByVal PlotXFeatureData As System.Object, _    ByVal PlotYFeatureData As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICosmosMotionStudyResults Dim PlotFeatureData As System.Object Dim PlotXFeatureData As System.Object Dim PlotYFeatureData As System.Object Dim value As System.Object   value = instance.InsertPlotFeature(PlotFeatureData, PlotXFeatureData, PlotYFeatureData) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertPlotFeature(     System.object PlotFeatureData,    System.object PlotXFeatureData,    System.object PlotYFeatureData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertPlotFeature(  &   System.Object^ PlotFeatureData, &   System.Object^ PlotXFeatureData, &   System.Object^ PlotYFeatureData ) ``` | |

#### Parameters

*PlotFeatureData*
:   Plot's feature data

*PlotXFeatureData*
:   Plot's x-axis feature data

*PlotYFeatureData*
:   Plot's y-axis feature data

#### Return Value

Feature

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CosmosMotionStudyResults::InsertPlotFeature.

# ![](dotnetimages/collapse.gif)Example

[Create Plots and Get Values (C#)](Create_Plots_and_Get_Values_Example_CSharp.htm)

[Create Plots and Get Values (VB.NET)](Create_Plots_and_Get_Values_Example_VBNET.htm)

[Create Plots and Get Values (VBA)](Create_Plots_and_Get_Values_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICosmosMotionStudyResults Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyResults.html)

[ICosmosMotionStudyResults Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.ICosmosMotionStudyResults_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0