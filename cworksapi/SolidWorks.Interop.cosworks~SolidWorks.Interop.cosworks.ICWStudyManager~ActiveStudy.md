<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~ActiveStudy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ActiveStudy Property (ICWStudyManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html) : ActiveStudy Property (ICWStudyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the index of the active study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ActiveStudy As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyManager Dim value As System.Integer   instance.ActiveStudy = value   value = instance.ActiveStudy ``` | |

| C# |  |
| --- | --- |
| ``` System.int ActiveStudy {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int ActiveStudy {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Index of the active study

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyManager::ActiveStudy.

# ![](dotnetimages/collapse.gif)Example

[Calculate Edge Weld Results (C#)](Calculate_Edge_Weld_Results_Example_CSharp.htm)

[Calculate Edge Weld Results (VB.NET)](Calculate_Edge_Weld_Results_Example_VBNET.htm)

[Calculate Edge Weld Results (VBA)](Calculate_Edge_Weld_Results_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html)

[ICWStudyManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager_members.html)

[ICWStudy::ActivateConfiguration Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~ActivateConfiguration.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0