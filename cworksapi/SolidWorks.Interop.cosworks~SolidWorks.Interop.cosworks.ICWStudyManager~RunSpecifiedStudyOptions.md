<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~RunSpecifiedStudyOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| RunSpecifiedStudyOptions Property (ICWStudyManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html) : RunSpecifiedStudyOptions Property (ICWStudyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the run and mesh option for studies run in batch mode.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property RunSpecifiedStudyOptions As CWRunSpecStudiesRunMeshOptions ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyManager Dim value As CWRunSpecStudiesRunMeshOptions   value = instance.RunSpecifiedStudyOptions ``` | |

| C# |  |
| --- | --- |
| ``` CWRunSpecStudiesRunMeshOptions RunSpecifiedStudyOptions {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property CWRunSpecStudiesRunMeshOptions^ RunSpecifiedStudyOptions {    CWRunSpecStudiesRunMeshOptions^ get(); } ``` | |

#### Property Value

[ICWRunSpecStudiesRunMeshOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyManager::RunSpecifiedStudyOptions.

# ![](dotnetimages/collapse.gif)Example

[Run Studies in Batch Mode (VBA)](Run_Studies_in_Batch_Mode_Example_VB.htm)

[Run Studies in Batch Mode (VB.NET)](Run_Studies_in_Batch_Mode_Example_VBNET.htm)

[Run Studies in Batch Mode (C#)](Run_Studies_in_Batch_Mode_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html)

[ICWStudyManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0