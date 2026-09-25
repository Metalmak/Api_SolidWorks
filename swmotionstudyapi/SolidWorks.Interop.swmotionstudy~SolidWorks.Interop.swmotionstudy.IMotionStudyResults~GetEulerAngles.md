<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyResults~GetEulerAngles.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| GetEulerAngles Method (IMotionStudyResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) > [IMotionStudyResults Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyResults.html) : GetEulerAngles Method (IMotionStudyResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Time*
:   Time

*Component*
:   Component

Gets the euler angles of the specified component at the specified time.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetEulerAngles( _    ByVal Time As System.Double, _    ByVal Component As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMotionStudyResults Dim Time As System.Double Dim Component As System.Object Dim value As System.Object   value = instance.GetEulerAngles(Time, Component) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetEulerAngles(     System.double Time,    System.object Component ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetEulerAngles(  &   System.double Time, &   System.Object^ Component ) ``` | |

#### Parameters

*Time*
:   Time

*Component*
:   Component

#### Return Value

Component's euler angles

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MotionStudyResults::GetEulerAngles.

# ![](dotnetimages/collapse.gif)See Also

####

[IMotionStudyResults Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyResults.html)

[IMotionStudyResults Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudyResults_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0