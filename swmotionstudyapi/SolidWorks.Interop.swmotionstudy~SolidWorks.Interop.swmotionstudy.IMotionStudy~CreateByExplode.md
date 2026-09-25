<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~CreateByExplode.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| CreateByExplode Method (IMotionStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) > [IMotionStudy Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy.html) : CreateByExplode Method (IMotionStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DeleteExistingPath*
:   True to delete any existing animation sequences, false to not

*Duration*
:   Length of time of the animation in seconds

*StartTime*
:   Time to start this animation (see Remarks)

Creates an animation in which a collapsed view of an assembly is exploded.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateByExplode( _    ByVal DeleteExistingPath As System.Boolean, _    ByVal Duration As System.Double, _    ByVal StartTime As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMotionStudy Dim DeleteExistingPath As System.Boolean Dim Duration As System.Double Dim StartTime As System.Double Dim value As System.Boolean   value = instance.CreateByExplode(DeleteExistingPath, Duration, StartTime) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateByExplode(     System.bool DeleteExistingPath,    System.double Duration,    System.double StartTime ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateByExplode(  &   System.bool DeleteExistingPath, &   System.double Duration, &   System.double StartTime ) ``` | |

#### Parameters

*DeleteExistingPath*
:   True to delete any existing animation sequences, false to not

*Duration*
:   Length of time of the animation in seconds

*StartTime*
:   Time to start this animation (see Remarks)

#### Return Value

True if the animation is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MotionStudy::CreateByExplode.

# ![](dotnetimages/collapse.gif)Example

[Duplicate, Delete, and Create Motion Study (C#)](Duplicate%2C_Delete%2C_and_Create_Motion_Study_Example_CSharp.htm)

[Duplicate, Delete, and Create Motion Study (VB.NET)](Duplicate%2C_Delete%2C_and_Create_Motion_Study_Example_VBNET.htm)

[Duplicate, Delete, and Create Motion Study (VBA)](Duplicate%2C_Delete%2C_and_Create_Motion_Study_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you have existing animation sequences, then the start time of this animation should account for the total time of all previous sequences. If this is a new animation sequence, set StartTime to 0 to start the animation immediately, or type a value to delay the start of the sequence.

Example:

' Precondition: Active document contains an exploded view of an assembly.

Option Explicit

Dim swApp As SldWorks.SldWorks

Dim swModel As SldWorks.ModelDoc2

Dim swModelDocExt As SldWorks.ModelDocExtension

Dim swMotionMgr As SwMotionStudy.MotionStudyManager

Dim swMotion As SwMotionStudy.MotionStudy

Dim boolstatus As Boolean

Sub main()

Set swApp = Application.SldWorks

'Active document contains an exploded view of an assembly

Set swModel = swApp.ActiveDoc

Set swModelDocExt = swModel.Extension

Set swMotionMgr = swModelDocExt.GetMotionStudyManager

' Create a new motion study

Set swMotion = swMotionMgr.CreateMotionStudy

' Delete any existing animation sequences,

' set the animation duration to 5 seconds, and play

' the animation immediately when IMotionStudy::Play is called

boolstatus = swMotion.CreateByExplode(True, 5, 0)

' Play the animation

swMotion.Play

End Sub

# ![](dotnetimages/collapse.gif)See Also

####

[IMotionStudy Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy.html)

[IMotionStudy Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy_members.html)

[IMotionStudy::CreateByCollapse Method](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~CreateByCollapse.html)

[IMotionStudy::CreateByRotateModel Method](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~CreateByRotateModel.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0