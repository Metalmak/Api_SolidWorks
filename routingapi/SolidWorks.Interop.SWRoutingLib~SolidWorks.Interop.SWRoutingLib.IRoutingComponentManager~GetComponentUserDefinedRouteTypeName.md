<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~GetComponentUserDefinedRouteTypeName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetComponentUserDefinedRouteTypeName Method (IRoutingComponentManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html) : GetComponentUserDefinedRouteTypeName Method (IRoutingComponentManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the name of the user-defined route for the active routing component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetComponentUserDefinedRouteTypeName() As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingComponentManager Dim value As System.String   value = instance.GetComponentUserDefinedRouteTypeName() ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetComponentUserDefinedRouteTypeName() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetComponentUserDefinedRouteTypeName(); ``` | |

#### Return Value

Name of the user-defined route for the active routing component

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RoutingComponentManager::GetComponentUserDefinedRouteTypeName.

# ![](dotnetimages/collapse.gif)Example

[Set User-defined Route (C#)](Set_User-defined_Route_Example_CSharp.htm)

[Set User-defined Route (VB.NET)](Set_User-defined_Route_Example_VBNET.htm)

[Set User-defined Route (VBA)](Set_User-defined_Route_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The name of a user-defined route for the active routing component is optional and intended for:

* air conditioning and other mechanical styles of ducting.* space planning.

Examples of names of user-defined route types are **HVAC**, **Ducting**, **Conveyors**, **Space** **Planning**, etc.

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html)

[IRoutingComponentManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager_members.html)

[IRoutingComponentManager::SetComponentUserDefinedRouteTypeName Method ()](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~SetComponentUserDefinedRouteTypeName.html)

[IRoutingComponentManager::GetComponentCrossSectionType Method ()](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~GetComponentCrossSectionType.html)

[IRoutingComponentManager::SetComponentCrossSectionType Method ()](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~SetComponentCrossSectionType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2015 FCS