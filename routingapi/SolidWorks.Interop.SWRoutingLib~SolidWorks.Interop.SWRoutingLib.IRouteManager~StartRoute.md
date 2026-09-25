<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~StartRoute.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| StartRoute Method (IRouteManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html) : StartRoute Method (IRouteManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Pathname*
:   Path and file name of the routing part from which to start a route or "" if using a selected connection point or a selected routing component

*ConfigName*
:   Configuration of the specified routing part from which to start the route or "" if using a selected connection point or a selected routing component

Starts a route from one of the following:

* selected connection point* selected routing component* specified routing part and configuration

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function StartRoute( _    ByVal Pathname As System.String, _    ByVal ConfigName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRouteManager Dim Pathname As System.String Dim ConfigName As System.String Dim value As System.Boolean   value = instance.StartRoute(Pathname, ConfigName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool StartRoute(     System.string Pathname,    System.string ConfigName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool StartRoute(  &   System.String^ Pathname, &   System.String^ ConfigName ) ``` | |

#### Parameters

*Pathname*
:   Path and file name of the routing part from which to start a route or "" if using a selected connection point or a selected routing component

*ConfigName*
:   Configuration of the specified routing part from which to start the route or "" if using a selected connection point or a selected routing component

#### Return Value

True if a route started, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RouteManager::StartRoute.

# ![](dotnetimages/collapse.gif)Example

[Start Route (VBA)](Start_Route_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Calling this method places the assembly in routing edit mode.

|  |  |
| --- | --- |
| **To exit...** | **Call...** |
| 1. Routing edit mode | [IRouteManager::ExitRoute](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~ExitRoute.html) |
| 2. Assembly edit mode | IAssemblyDoc::EditAssembly |

# ![](dotnetimages/collapse.gif)See Also

####

[IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html)

[IRouteManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager_members.html)

[IRouteManager::AddToRoute](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~AddToRoute.html)

[IRouteManager::EditRoute](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~EditRoute.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2013 FCS