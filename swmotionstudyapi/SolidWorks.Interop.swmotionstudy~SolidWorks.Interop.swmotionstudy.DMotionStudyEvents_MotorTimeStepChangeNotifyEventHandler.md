<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_MotorTimeStepChangeNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| DMotionStudyEvents\_MotorTimeStepChangeNotifyEventHandler Delegate (SolidWorks.Interop.swmotionstudy) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) : DMotionStudyEvents\_MotorTimeStepChangeNotifyEventHandler Delegate (SolidWorks.Interop.swmotionstudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Motor*
:   Motor name

*Time*
:   Time

*MotorSpeed*
:   New motor speed

Fired when a motion study is [calculated](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.IMotionStudy~Calculate.html) and there are external motors.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DMotionStudyEvents_MotorTimeStepChangeNotifyEventHandler( _    ByVal Motor As System.String, _    ByVal Time As System.Double, _    ByRef MotorSpeed As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DMotionStudyEvents_MotorTimeStepChangeNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DMotionStudyEvents_MotorTimeStepChangeNotifyEventHandler(     System.string Motor,    System.double Time,    ref System.double MotorSpeed ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DMotionStudyEvents_MotorTimeStepChangeNotifyEventHandler(  &   System.String^ Motor, &   System.double Time, &   System.double% MotorSpeed ) ``` | |

#### Parameters

*Motor*
:   Motor name

*Time*
:   Time

*MotorSpeed*
:   New motor speed

# ![](dotnetimages/collapse.gif)Visual Basic Application (VBA) Syntax

See MotorTimeStepChangeNotify Event (MotionStudy).

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, then use [swMotionStudyMotorTimeStepChangeNotify](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.swMotionStudyNotify_e.html) to register for this notification.

You can implement any motion law after catching this event. The return value is a double that specifies the new motor speed. This event is called at every major time step from ADAMS.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 SP01, Revision Number 16.1