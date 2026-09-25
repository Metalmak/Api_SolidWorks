<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~GetRouteComponentTypeSetThrRLM.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetRouteComponentTypeSetThrRLM Method (IRoutingComponentManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html) : GetRouteComponentTypeSetThrRLM Method (IRoutingComponentManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether the type of the active routing component is set through the Routing Library Manager.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetRouteComponentTypeSetThrRLM() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingComponentManager Dim value As System.Boolean   value = instance.GetRouteComponentTypeSetThrRLM() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetRouteComponentTypeSetThrRLM() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetRouteComponentTypeSetThrRLM(); ``` | |

#### Return Value

True if the type is set through the Routing Library Manager, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RoutingComponentManager::GetRouteComponentTypeSetThrRLM.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Routing Component Properties Example (C#)](Get_and_Set_Routing_Component_Properties_Example_CSharp.htm)

[Get and Set Routing Component Properties Example (VB.NET)](Get_and_Set_Routing_Component_Properties_Example_VBNET.htm)

[Get and Set Routing Component Properties Example (VBA)](Get_and_Set_Routing_Component_Properties_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html)

[IRoutingComponentManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager_members.html)

[IRoutingComponentManager::SetRouteComponentTypeSetThrRLM Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~SetRouteComponentTypeSetThrRLM.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2011 FCS