<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~Duplicate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| Duplicate Method (IMotionStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) > [IMotionStudy Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy.html) : Duplicate Method (IMotionStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Creates a new motion study based on the specified motion study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Duplicate() As MotionStudy ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMotionStudy Dim value As MotionStudy   value = instance.Duplicate() ``` | |

| C# |  |
| --- | --- |
| ``` MotionStudy Duplicate() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` MotionStudy^ Duplicate(); ``` | |

#### Return Value

Duplicated [motion study](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.IMotionStudy.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MotionStudy::Duplicate.

# ![](dotnetimages/collapse.gif)Example

[Duplicate, Delete, and Create Motion Study (C#)](Duplicate%2C_Delete%2C_and_Create_Motion_Study_Example_CSharp.htm)

[Duplicate, Delete, and Create Motion Study (VB.NET)](Duplicate%2C_Delete%2C_and_Create_Motion_Study_Example_VBNET.htm)

[Duplicate, Delete, and Create Motion Study (VBA)](Duplicate%2C_Delete%2C_and_Create_Motion_Study_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The name of the duplicated motion study is Motion Study followed by a number. The number for the duplicated motion study is determined by incrementing the number of the Motion Study with the highest number by 1 and adding that number to the duplicated motion study's name (e.g., only Motion Study 1 exists; duplicated motion study's name is Motion Study 2).

# ![](dotnetimages/collapse.gif)See Also

####

[IMotionStudy Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy.html)

[IMotionStudy Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0