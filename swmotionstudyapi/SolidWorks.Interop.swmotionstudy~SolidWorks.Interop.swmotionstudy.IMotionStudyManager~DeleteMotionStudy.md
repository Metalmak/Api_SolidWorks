<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyManager~DeleteMotionStudy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| DeleteMotionStudy Method (IMotionStudyManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) > [IMotionStudyManager Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyManager.html) : DeleteMotionStudy Method (IMotionStudyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MotionStudyName*
:   Name of motion study to delete

Deletes the specified motion study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DeleteMotionStudy( _    ByVal MotionStudyName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMotionStudyManager Dim MotionStudyName As System.String Dim value As System.Boolean   value = instance.DeleteMotionStudy(MotionStudyName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool DeleteMotionStudy(     System.string MotionStudyName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool DeleteMotionStudy(  &   System.String^ MotionStudyName ) ``` | |

#### Parameters

*MotionStudyName*
:   Name of motion study to delete

#### Return Value

True if the motion study is deleted, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MotionStudyManager::DeleteMotionStudy.

# ![](dotnetimages/collapse.gif)Example

[Create Motion Studies (VBA)](Create_Motion_Studies_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IMotionStudyManager Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyManager.html)

[IMotionStudyManager Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyManager_members.html)

[IMotionStudyManager::CreateMotionStudy Method](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyManager~CreateMotionStudy.html)

[IMotionStudyManager::GetMotionStudy Method](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyManager~GetMotionStudy.html)

[IMotionStudyManager::GetMotionStudyCount Method](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyManager~GetMotionStudyCount.html)

[IMotionStudyManager::GetMotionStudyNames Method](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyManager~GetMotionStudyNames.html)

[IMotionStudyManager::IGetMotionStudyNames Method](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyManager~IGetMotionStudyNames.html)

[IMotionStudyManager::ActivateMotionStudy Method](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyManager~ActivateMotionStudy.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0