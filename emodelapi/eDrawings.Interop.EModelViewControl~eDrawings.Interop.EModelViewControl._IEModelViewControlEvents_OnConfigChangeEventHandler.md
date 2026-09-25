<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnConfigChangeEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| \_IEModelViewControlEvents\_OnConfigChangeEventHandler Delegate (eDrawings.Interop.EModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) : \_IEModelViewControlEvents\_OnConfigChangeEventHandler Delegate (eDrawings.Interop.EModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ConfigId*
:   Configuration ID

Fired when the specified configuration changes.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Sub _IEModelViewControlEvents_OnConfigChangeEventHandler( _    ByVal ConfigId As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New _IEModelViewControlEvents_OnConfigChangeEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnConfigChangeEventHandler(     System.int ConfigId ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnConfigChangeEventHandler(  &   System.int ConfigId ) ``` | |

#### Parameters

*ConfigId*
:   Configuration ID

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See [OnConfigChange Event (EModelViewControl).](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnConfigChangeEventHandler.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings 2019 SP0