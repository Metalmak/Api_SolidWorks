<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.DMotionStudyEvents_PartCollideNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| DMotionStudyEvents\_PartCollideNotifyEventHandler Delegate (SolidWorks.Interop.swmotionstudy) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) : DMotionStudyEvents\_PartCollideNotifyEventHandler Delegate (SolidWorks.Interop.swmotionstudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Time*
:   Time of collision

*Component1*
:   Component 1

*Component2*
:   Component 2

*Vector1*
:   Point on Component1

*Vector2*
:   :   Point on Component 2

*SurfaceNormal1*
:   :   Surface normal of Component 1

*SurfaceNormal2*
:   :   Surface normal of Component 2

Fired when a collision between two components occurs.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DMotionStudyEvents_PartCollideNotifyEventHandler( _    ByVal Time As System.Double, _    ByVal Component1 As System.Object, _    ByVal Component2 As System.Object, _    ByVal Vector1 As System.Object, _    ByVal Vector2 As System.Object, _    ByVal SurfaceNormal1 As System.Object, _    ByVal SurfaceNormal2 As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DMotionStudyEvents_PartCollideNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DMotionStudyEvents_PartCollideNotifyEventHandler(     System.double Time,    System.object Component1,    System.object Component2,    System.object Vector1,    System.object Vector2,    System.object SurfaceNormal1,    System.object SurfaceNormal2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DMotionStudyEvents_PartCollideNotifyEventHandler(  &   System.double Time, &   System.Object^ Component1, &   System.Object^ Component2, &   System.Object^ Vector1, &   System.Object^ Vector2, &   System.Object^ SurfaceNormal1, &   System.Object^ SurfaceNormal2 ) ``` | |

#### Parameters

*Time*
:   Time of collision

*Component1*
:   Component 1

*Component2*
:   Component 2

*Vector1*
:   Point on Component1

*Vector2*
:   :   Point on Component 2

*SurfaceNormal1*
:   :   Surface normal of Component 1

*SurfaceNormal2*
:   :   Surface normal of Component 2

# ![](dotnetimages/collapse.gif)Visual Basic Application (VBA) Syntax

See PartCollideNotify Event (MotionStudy).

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, then use [swMotionStudyPartCollideNotify](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.swMotionStudyNotify_e.html) to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 SP01, Revision Number 16.1