<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~RunSpecifiedStudyByName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| RunSpecifiedStudyByName Method (ICWStudyManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html) : RunSpecifiedStudyByName Method (ICWStudyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ErrorCode*
:   Error code as defined in [swsRunStudiesErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRunStudiesErrorCode_e.html)

Runs specified studies in batch mode.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RunSpecifiedStudyByName( _    ByRef ErrorCode As System.Integer _ ) As CWRunStudiesResults ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyManager Dim ErrorCode As System.Integer Dim value As CWRunStudiesResults   value = instance.RunSpecifiedStudyByName(ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWRunStudiesResults RunSpecifiedStudyByName(     out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWRunStudiesResults^ RunSpecifiedStudyByName(  &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*ErrorCode*
:   Error code as defined in [swsRunStudiesErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRunStudiesErrorCode_e.html)

#### Return Value

[ICWRunStudiesResults](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunStudiesResults.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyManager::RunSpecifiedStudyByName.

# ![](dotnetimages/collapse.gif)Example

[Run Studies in Batch Mode (VBA)](Run_Studies_in_Batch_Mode_Example_VB.htm)

[Run Studies in Batch Mode (VB.NET)](Run_Studies_in_Batch_Mode_Example_VBNET.htm)

[Run Studies in Batch Mode (C#)](Run_Studies_in_Batch_Mode_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, set the run and mesh options for the study using [ICWStudyManager::RunSpecifiedStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~RunSpecifiedStudyOptions.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html)

[ICWStudyManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager_members.html)

[ICWStudyManager::RunAllStudies Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~RunAllStudies.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0