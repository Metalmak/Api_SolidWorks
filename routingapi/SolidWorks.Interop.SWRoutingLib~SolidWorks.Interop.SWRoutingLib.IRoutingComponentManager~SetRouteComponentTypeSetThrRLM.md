<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~SetRouteComponentTypeSetThrRLM.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| SetRouteComponentTypeSetThrRLM Method (IRoutingComponentManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html) : SetRouteComponentTypeSetThrRLM Method (IRoutingComponentManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ComponentType*
:   True to indicate that the type of the component is set through the Routing Library Manager, false to indicate that the type is not set through the Routing Library Manager

Sets whether the type of the active routing component is set through the Routing Library Manager.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetRouteComponentTypeSetThrRLM( _    ByVal ComponentType As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingComponentManager Dim ComponentType As System.Boolean   instance.SetRouteComponentTypeSetThrRLM(ComponentType) ``` | |

| C# |  |
| --- | --- |
| ``` void SetRouteComponentTypeSetThrRLM(     System.bool ComponentType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetRouteComponentTypeSetThrRLM(  &   System.bool ComponentType ) ``` | |

#### Parameters

*ComponentType*
:   True to indicate that the type of the component is set through the Routing Library Manager, false to indicate that the type is not set through the Routing Library Manager

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RoutingComponentManager::SetRouteComponentTypeSetThrRLM.

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html)

[IRoutingComponentManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager_members.html)

[IRoutingComponentManager::GetRouteComponentTypeSetThrRLM Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~GetRouteComponentTypeSetThrRLM.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2011 FCS