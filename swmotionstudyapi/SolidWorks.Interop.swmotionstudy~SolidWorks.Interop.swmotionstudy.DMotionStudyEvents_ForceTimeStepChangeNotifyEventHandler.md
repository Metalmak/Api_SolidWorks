<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_ForceTimeStepChangeNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| DMotionStudyEvents\_ForceTimeStepChangeNotifyEventHandler Delegate (SolidWorks.Interop.swmotionstudy) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) : DMotionStudyEvents\_ForceTimeStepChangeNotifyEventHandler Delegate (SolidWorks.Interop.swmotionstudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Force*
:   Force name

*Time*
:   Time

*ForceMagnitude*
:   New force or torque magnitude

Fired when a motion study is [calculated](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.IMotionStudy~Calculate.html) and there are external forces.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DMotionStudyEvents_ForceTimeStepChangeNotifyEventHandler( _    ByVal Force As System.String, _    ByVal Time As System.Double, _    ByRef ForceMagnitude As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DMotionStudyEvents_ForceTimeStepChangeNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DMotionStudyEvents_ForceTimeStepChangeNotifyEventHandler(     System.string Force,    System.double Time,    ref System.double ForceMagnitude ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DMotionStudyEvents_ForceTimeStepChangeNotifyEventHandler(  &   System.String^ Force, &   System.double Time, &   System.double% ForceMagnitude ) ``` | |

#### Parameters

*Force*
:   Force name

*Time*
:   Time

*ForceMagnitude*
:   New force or torque magnitude

# ![](dotnetimages/collapse.gif)Visual Basic Application (VBA) Syntax

See ForceTimeStepChangeNotify Event (MotionStudy).

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, then use [swMotionStudyForceTimeStepChangeNotify](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.swMotionStudyNotify_e.html) to register for this notification.

You can implement any force law after catching this event. The return value is a double that specifies the new force or torque magnitude. This event is called at every major time step from ADAMS.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 SP01, Revision Number 16.1