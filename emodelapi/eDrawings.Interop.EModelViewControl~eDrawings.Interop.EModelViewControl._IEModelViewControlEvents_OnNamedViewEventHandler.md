<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnNamedViewEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| \_IEModelViewControlEvents\_OnNamedViewEventHandler Delegate (eDrawings.Interop.EModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) : \_IEModelViewControlEvents\_OnNamedViewEventHandler Delegate (eDrawings.Interop.EModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NamedViewId*
:   Named views:

    * 0xDDDD = Front View* 0xDDDE = Back view* 0xDDDF = Left view* 0xDDED = Right view* 0xDDEE = Top view* 0xDDEF = Bottom view* 0xDDFD = Isometric view* 0xDDFE = Normal view

Fired when a named view has been selected.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Sub _IEModelViewControlEvents_OnNamedViewEventHandler( _    ByVal NamedViewId As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New _IEModelViewControlEvents_OnNamedViewEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnNamedViewEventHandler(     System.int NamedViewId ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnNamedViewEventHandler(  &   System.int NamedViewId ) ``` | |

#### Parameters

*NamedViewId*
:   Named views:

    * 0xDDDD = Front View* 0xDDDE = Back view* 0xDDDF = Left view* 0xDDED = Right view* 0xDDEE = Top view* 0xDDEF = Bottom view* 0xDDFD = Isometric view* 0xDDFE = Normal view

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See OnNamedView Event (EModelViewControl).

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2014 SP1