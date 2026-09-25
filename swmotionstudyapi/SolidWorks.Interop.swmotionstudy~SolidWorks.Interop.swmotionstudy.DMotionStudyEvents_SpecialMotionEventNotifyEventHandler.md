<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_SpecialMotionEventNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| DMotionStudyEvents\_SpecialMotionEventNotifyEventHandler Delegate (SolidWorks.Interop.swmotionstudy) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) : DMotionStudyEvents\_SpecialMotionEventNotifyEventHandler Delegate (SolidWorks.Interop.swmotionstudy) |

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

*EventType*
:   Motion-related special event as defined in [swSpecialMotionEventType\_e](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.swSpecialMotionEventType_e.html)

Fired for motion-related special events, such as contacts.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DMotionStudyEvents_SpecialMotionEventNotifyEventHandler( _    ByVal Time As System.Double, _    ByVal EventType As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DMotionStudyEvents_SpecialMotionEventNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DMotionStudyEvents_SpecialMotionEventNotifyEventHandler(     System.double Time,    System.int EventType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DMotionStudyEvents_SpecialMotionEventNotifyEventHandler(  &   System.double Time, &   System.int EventType ) ``` | |

#### Parameters

*Time*
:   Time

*EventType*
:   Motion-related special event as defined in [swSpecialMotionEventType\_e](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.swSpecialMotionEventType_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic Application (VBA) Syntax

See SpecialMotionEventNotify Event (MotionStudy).

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, then use [swMotionStudySpecialEventNotify](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.swMotionStudyNotify_e.html) to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0