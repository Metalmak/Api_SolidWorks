<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~GetComponentCrossSectionType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetComponentCrossSectionType Method (IRoutingComponentManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html) : GetComponentCrossSectionType Method (IRoutingComponentManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the type of cross section for a user-defined route for the active routing component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetComponentCrossSectionType() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingComponentManager Dim value As System.Integer   value = instance.GetComponentCrossSectionType() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetComponentCrossSectionType() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetComponentCrossSectionType(); ``` | |

#### Return Value

Type of cross section for a user-defined route for the active routing component as defined in [swComponentCrossSectionType\_e](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.swComponentCrossSectionType_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RoutingComponentManager::GetComponentCrossSectionType.

# ![](dotnetimages/collapse.gif)Example

[Set User-defined Route (C#)](Set_User-defined_Route_Example_CSharp.htm)

[Set User-defined Route (VB.NET)](Set_User-defined_Route_Example_VBNET.htm)

[Set User-defined Route (VBA)](Set_User-defined_Route_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html)

[IRoutingComponentManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager_members.html)

[IRoutingComponentManager::SetComponentCrossSectionType Method ()](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~SetComponentCrossSectionType.html)

[IRoutingComponentManager::GetComponentUserDefinedRouteTypeName Method ()](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~GetComponentUserDefinedRouteTypeName.html)

[IRoutingComponentManager::SetComponentUserDefinedRouteTypeName Method ()](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~SetComponentUserDefinedRouteTypeName.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2015 FCS