<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~SetComponentRouteTypeToCustomProperty.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| SetComponentRouteTypeToCustomProperty Method (IRoutingComponentManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html) : SetComponentRouteTypeToCustomProperty Method (IRoutingComponentManager) |

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

Sets the route type for the custom property for the active routing component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetComponentRouteTypeToCustomProperty( _    ByVal RouteType As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingComponentManager Dim RouteType As System.Integer   instance.SetComponentRouteTypeToCustomProperty(RouteType) ``` | |

| C# |  |
| --- | --- |
| ``` void SetComponentRouteTypeToCustomProperty(     System.int RouteType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetComponentRouteTypeToCustomProperty(  &   System.int RouteType ) ``` | |

#### Parameters

*RouteType*
:   Type of route as defined in [swComponentRouteType\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swComponentRouteType_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RoutingComponentManager::SetComponentRouteTypeToCustomProperty.

# ![](dotnetimages/collapse.gif)Example

[Set User-defined Route (C#)](Set_User-defined_Route_Example_CSharp.htm)

[Set User-defined Route (VB.NET)](Set_User-defined_Route_Example_VBNET.htm)

[Set User-defined Route (VBA)](Set_User-defined_Route_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html)

[IRoutingComponentManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager_members.html)

[IRoutingComponentManager::GetComponentRouteTypeFromCustomProperty Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~GetComponentRouteTypeFromCustomProperty.html)

[IRoutingComponentManager::GetComponentRouteType Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~GetComponentRouteType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2013 FCS