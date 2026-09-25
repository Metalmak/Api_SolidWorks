<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~AddToRoute.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| AddToRoute Method (IRouteManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html) : AddToRoute Method (IRouteManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Creates a route from one or more selected connection points or on the connection points of a selected routing component in a routing assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddToRoute() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRouteManager Dim value As System.Boolean   value = instance.AddToRoute() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddToRoute() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddToRoute(); ``` | |

#### Return Value

True if a route is added, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RouteManager::AddToRoute.

# ![](dotnetimages/collapse.gif)Example

[Add to Route (VBA)](Add_to_Route_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must call [IRouteManager::EditRoute](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~EditRoute.html) to place the routing assembly in edit mode.

|  |  |
| --- | --- |
| **To exit...** | **Call...** |
| 1. Routing edit mode | [IRouteManager::ExitRoute](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~ExitRoute.html) |
| 2. Assembly edit mode | IAssemblyDoc::EditAssembly |

# ![](dotnetimages/collapse.gif)See Also

####

[IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html)

[IRouteManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager_members.html)

[IRouteManager::StartRoute](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~StartRoute.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2013 FCS