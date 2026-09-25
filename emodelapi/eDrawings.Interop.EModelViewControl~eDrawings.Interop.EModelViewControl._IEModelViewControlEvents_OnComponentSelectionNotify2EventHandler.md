<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnComponentSelectionNotify2EventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| \_IEModelViewControlEvents\_OnComponentSelectionNotify2EventHandler Delegate (eDrawings.Interop.EModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) : \_IEModelViewControlEvents\_OnComponentSelectionNotify2EventHandler Delegate (eDrawings.Interop.EModelViewControl) |

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

*ComponentConfigName*
:   Component configuration name

*XCoordinate*
:   x coordinate of cursor

*YCoordinate*
:   y coordinate of cursor

Fired when a component is selected.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Sub _IEModelViewControlEvents_OnComponentSelectionNotify2EventHandler( _    ByVal ComponentName As System.String, _    ByVal ComponentConfigName As System.String, _    ByVal XCoordinate As System.Integer, _    ByVal YCoordinate As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New _IEModelViewControlEvents_OnComponentSelectionNotify2EventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnComponentSelectionNotify2EventHandler(     System.string ComponentName,    System.string ComponentConfigName,    System.int XCoordinate,    System.int YCoordinate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnComponentSelectionNotify2EventHandler(  &   System.String^ ComponentName, &   System.String^ ComponentConfigName, &   System.int XCoordinate, &   System.int YCoordinate ) ``` | |

#### Parameters

*ComponentName*
:   Component name

*ComponentConfigName*
:   Component configuration name

*XCoordinate*
:   x coordinate of cursor

*YCoordinate*
:   y coordinate of cursor

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See OnComponentSelectionNotify2 Event (EModelViewControl).

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2013 SP0