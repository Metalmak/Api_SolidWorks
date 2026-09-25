<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~DeleteAllDefaultStaticStudyPlots.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| DeleteAllDefaultStaticStudyPlots Method (ICWModelDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) : DeleteAllDefaultStaticStudyPlots Method (ICWModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Deletes all default static study plots from this model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DeleteAllDefaultStaticStudyPlots() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWModelDoc Dim value As System.Integer   value = instance.DeleteAllDefaultStaticStudyPlots() ``` | |

| C# |  |
| --- | --- |
| ``` System.int DeleteAllDefaultStaticStudyPlots() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int DeleteAllDefaultStaticStudyPlots(); ``` | |

#### Return Value

Error code as defined in [swsResultPlotDelete\_ErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotDelete_ErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWModelDoc::DeleteAllDefaultStaticStudyPlots.

# ![](dotnetimages/collapse.gif)Example

[Create Plots for a Static Study (VBA)](Create_Plots_for_Static_Study_Example_VB.htm)

[Create Plots for a Static Study (VB.NET)](Create_Plots_for_Static_Study_Example_VBNET.htm)

[Create Plots for a Static Study (C#)](Create_Plots_for_Static_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html)

[ICWModelDoc Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc_members.html)

[ICWModelDoc::AddDefaultStaticStudyPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~AddDefaultStaticStudyPlot.html)

[ICWModelDoc::DeleteDefaultStaticStudyPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~DeleteDefaultStaticStudyPlot.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0