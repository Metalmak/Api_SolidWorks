<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~GetTimeTakenForInputPhase.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetTimeTakenForInputPhase Method (ICWStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html) : GetTimeTakenForInputPhase Method (ICWStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the time taken for the input phase of this static study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetTimeTakenForInputPhase() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudy Dim value As System.Integer   value = instance.GetTimeTakenForInputPhase() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetTimeTakenForInputPhase() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetTimeTakenForInputPhase(); ``` | |

#### Return Value

Time taken in seconds for the input phase of this static study

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudy::GetTimeTakenForInputPhase.

# ![](dotnetimages/collapse.gif)Example

[Create Plots for Static Study (VBA)](Create_Plots_for_Static_Study_Example_VB.htm)

[Create Plots for Static Study (VB.NET)](Create_Plots_for_Static_Study_Example_VBNET.htm)

[Create Plots for Static Study (C#)](Create_Plots_for_Static_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for static studies.

*model\_name***-***study\_name***.out** is created after the study is analyzed and contains this time taken for the input phase. Check the location of this file in the results folder that is configered in **Simulation > Options > Default Options**.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudy Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy_members.html)

[ICWStudy::GetTimeTakenForGapIterationsAndContactOperations Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~GetTimeTakenForGapIterationsAndContactOperations.html)

[ICWStudy::GetTimeTakenForInputDataTransferFromDatabase Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~GetTimeTakenForInputDataTransferFromDatabase.html)

[ICWStudy::GetTotalSolutionTime Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~GetTotalSolutionTime.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0