<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnModifySceneEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| \_IEModelViewControlEvents\_OnModifySceneEventHandler Delegate (eDrawings.Interop.EModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) : \_IEModelViewControlEvents\_OnModifySceneEventHandler Delegate (eDrawings.Interop.EModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModifyEvent*
:   Modification event bitmask:

    * 1 or 0x001 = Hide/Show* 2 or 0x002 = Rotate* 4 or 0x004 = Pan* 8 or 0x008 = Zoom* 16 or 0x010 = MakeTransparent* 32 or 0x020 = Next* 64 or 0x040 = Projection* 128 or 0x080 = LayerChange* 256 or 0x100 = DisplayStateChange

Fired when a scene is modified.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Sub _IEModelViewControlEvents_OnModifySceneEventHandler( _    ByVal ModifyEvent As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New _IEModelViewControlEvents_OnModifySceneEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnModifySceneEventHandler(     System.int ModifyEvent ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnModifySceneEventHandler(  &   System.int ModifyEvent ) ``` | |

#### Parameters

*ModifyEvent*
:   Modification event bitmask:

    * 1 or 0x001 = Hide/Show* 2 or 0x002 = Rotate* 4 or 0x004 = Pan* 8 or 0x008 = Zoom* 16 or 0x010 = MakeTransparent* 32 or 0x020 = Next* 64 or 0x040 = Projection* 128 or 0x080 = LayerChange* 256 or 0x100 = DisplayStateChange

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See OnModifyScene Event (EModelViewControl).

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2015 SP0