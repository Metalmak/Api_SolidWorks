<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~SetRouteTypeAndSubRouteType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| SetRouteTypeAndSubRouteType Method (IRoutingComponentManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html) : SetRouteTypeAndSubRouteType Method (IRoutingComponentManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RouteType*
:   Type of route as defined in [swComponentRouteType\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swComponentRouteType_e.html)

*SubRouteType*
:   Type of electrical sub-route as defined in [swComponentRouteType\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swComponentRouteType_e.html); only valid if RouteType is Electrical or 3

Sets the route type and sub-type for the connection point of the active routing component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetRouteTypeAndSubRouteType( _    ByVal RouteType As System.Integer, _    ByVal SubRouteType As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingComponentManager Dim RouteType As System.Integer Dim SubRouteType As System.Integer   instance.SetRouteTypeAndSubRouteType(RouteType, SubRouteType) ``` | |

| C# |  |
| --- | --- |
| ``` void SetRouteTypeAndSubRouteType(     System.int RouteType,    System.int SubRouteType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetRouteTypeAndSubRouteType(  &   System.int RouteType, &   System.int SubRouteType ) ``` | |

#### Parameters

*RouteType*
:   Type of route as defined in [swComponentRouteType\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swComponentRouteType_e.html)

*SubRouteType*
:   Type of electrical sub-route as defined in [swComponentRouteType\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swComponentRouteType_e.html); only valid if RouteType is Electrical or 3

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RoutingComponentManager::SetRouteTypeAndSubRouteType.

# ![](dotnetimages/collapse.gif)Remarks

When a connection point is added to a routing component in the Routing Component Wizard, the **Connection Point** PropertyManager page is launched. This method sets the route type and sub-type fields on that page.

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html)

[IRoutingComponentManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2011 FCS