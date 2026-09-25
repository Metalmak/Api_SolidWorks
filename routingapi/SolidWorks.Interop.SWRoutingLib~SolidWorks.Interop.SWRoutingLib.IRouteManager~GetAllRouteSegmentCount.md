<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~GetAllRouteSegmentCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetAllRouteSegmentCount Method (IRouteManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html) : GetAllRouteSegmentCount Method (IRouteManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the number of route segments for active route.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetAllRouteSegmentCount() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRouteManager Dim value As System.Integer   value = instance.GetAllRouteSegmentCount() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetAllRouteSegmentCount() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetAllRouteSegmentCount(); ``` | |

#### Return Value

Number of route segments for active route

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RouteManager::GetAllRouteSegmentCount.

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [IRouteManager::IGetAllRouteSegmentIDs](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~IGetAllRouteSegmentIDs.html) to get the size of the array for that method.

# ![](dotnetimages/collapse.gif)See Also

####

[IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html)

[IRouteManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager_members.html)

[IRouteManager::GetAllRouteSegmentIDs Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~GetAllRouteSegmentIDs.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2008 FCS