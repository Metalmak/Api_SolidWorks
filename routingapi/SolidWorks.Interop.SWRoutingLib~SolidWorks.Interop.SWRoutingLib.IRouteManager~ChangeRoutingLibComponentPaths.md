<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~ChangeRoutingLibComponentPaths.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| ChangeRoutingLibComponentPaths Method (IRouteManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html) : ChangeRoutingLibComponentPaths Method (IRouteManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*oldLibPaths*
:   Old routing library paths

*newLibPaths*
:   New routing library paths

Replaces the old routing library paths with new routing library paths.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ChangeRoutingLibComponentPaths( _    ByVal oldLibPaths As System.Object, _    ByVal newLibPaths As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRouteManager Dim oldLibPaths As System.Object Dim newLibPaths As System.Object   instance.ChangeRoutingLibComponentPaths(oldLibPaths, newLibPaths) ``` | |

| C# |  |
| --- | --- |
| ``` void ChangeRoutingLibComponentPaths(     System.object oldLibPaths,    System.object newLibPaths ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ChangeRoutingLibComponentPaths(  &   System.Object^ oldLibPaths, &   System.Object^ newLibPaths ) ``` | |

#### Parameters

*oldLibPaths*
:   Old routing library paths

*newLibPaths*
:   New routing library paths

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RouteManager::ChangeRoutingLibComponentPaths.

# ![](dotnetimages/collapse.gif)See Also

####

[IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html)

[IRouteManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2007 SP1