<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnComponentMouseOverNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| \_IEModelViewControlEvents\_OnComponentMouseOverNotifyEventHandler Delegate (eDrawings.Interop.EModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) : \_IEModelViewControlEvents\_OnComponentMouseOverNotifyEventHandler Delegate (eDrawings.Interop.EModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ComponentName*
:   Component name

*XCoordinate*
:   x coordinate of cursor

*YCoordinate*
:   y coordinate of cursor

Obsolete. Superseded by [IEModelViewControlEvents::OnComponentMouseOverNotify2](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnComponentMouseOverNotify2EventHandler.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Sub _IEModelViewControlEvents_OnComponentMouseOverNotifyEventHandler( _    ByVal ComponentName As System.String, _    ByVal XCoordinate As System.Integer, _    ByVal YCoordinate As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New _IEModelViewControlEvents_OnComponentMouseOverNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnComponentMouseOverNotifyEventHandler(     System.string ComponentName,    System.int XCoordinate,    System.int YCoordinate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnComponentMouseOverNotifyEventHandler(  &   System.String^ ComponentName, &   System.int XCoordinate, &   System.int YCoordinate ) ``` | |

#### Parameters

*ComponentName*
:   Component name

*XCoordinate*
:   x coordinate of cursor

*YCoordinate*
:   y coordinate of cursor

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See OnComoponentMouseOverNotify Event (EModelViewControl).

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2005 SP0