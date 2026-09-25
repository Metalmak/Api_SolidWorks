<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_OutputTimeStepChangeNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| DMotionStudyEvents\_OutputTimeStepChangeNotifyEventHandler Delegate (SolidWorks.Interop.swmotionstudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) : DMotionStudyEvents\_OutputTimeStepChangeNotifyEventHandler Delegate (SolidWorks.Interop.swmotionstudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Time*
:   Output time when the event is fired

Fired at every integrator or output time step when a motion simulation is occurring.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DMotionStudyEvents_OutputTimeStepChangeNotifyEventHandler( _    ByVal Time As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DMotionStudyEvents_OutputTimeStepChangeNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DMotionStudyEvents_OutputTimeStepChangeNotifyEventHandler(     System.double Time ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DMotionStudyEvents_OutputTimeStepChangeNotifyEventHandler(  &   System.double Time ) ``` | |

#### Parameters

*Time*
:   Output time when the event is fired

# ![](dotnetimages/collapse.gif)Visual Basic Application (VBA) Syntax

See OutputTimeStepChangeNotify Event (MotionStudy).

# ![](dotnetimages/collapse.gif)Example

[Fire Events for External Output Time Step Changes (C#)](Fire_Events_for_External_Output_Time_Step_Changes_Example_CSharp.htm)

[Fire Events for External Output Time Step Changes (VB.NET)](Fire_Events_for_External_Output_Time_Step_Changes_Example_VBNET.htm)

[Fire Events for External Output Time Step Changes (VBA)](Fire_Events_for_External_Output_Time_Step_Changes_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

When the motion simulation is occurring, the solver takes two types of time steps:

* integrator* output

Integrator time steps are taken during the solve; thus, it is not guaranteed that the solver will actually converge at that step. Output time steps are taken after the solver has converged. By default, the OutputTimeStepChangeNotify event is fired at integrator time steps. If you want to fire this event at output time steps, then set [IMotionStudy::SetFireOutputTimeStepEvents](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.IMotionStudy~SetFireOutputTimeStepEvents.html) to true.

If developing a C++ application, then use [swMotionStudyOutputTimeStepChangeNotify](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.swMotionStudyNotify_e.html) to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0