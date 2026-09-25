<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager~GetRoutingStringValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetRoutingStringValue Method (IRoutingComponentManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html) : GetRoutingStringValue Method (IRoutingComponentManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StringID*
:   Integer representing one of the aspects of the routing component as follows:

    * 0 - pipe sketch* 1 - inner diameter* 2 - outer diameter* 3 - filter sketch* 4 - nominal diameter* 5 - length extrusion* 6 - specification* 7 - pipe identifier* 8 - elbow arc* 9 - bend angle* 10 - bend radius* 11 - BOM elbow angle* 12 - BOM pipe length* 13 - BOM total pipe length* 14 - vertical axis* 15 - axis of rotation* 16 - clip axis* 17 - BOM route length* 18 - ignore BOM value

Gets the string value for the specified aspect of the active routing component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetRoutingStringValue( _    ByVal StringID As System.Integer _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingComponentManager Dim StringID As System.Integer Dim value As System.String   value = instance.GetRoutingStringValue(StringID) ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetRoutingStringValue(     System.int StringID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetRoutingStringValue(  &   System.int StringID ) ``` | |

#### Parameters

*StringID*
:   Integer representing one of the aspects of the routing component as follows:

    * 0 - pipe sketch* 1 - inner diameter* 2 - outer diameter* 3 - filter sketch* 4 - nominal diameter* 5 - length extrusion* 6 - specification* 7 - pipe identifier* 8 - elbow arc* 9 - bend angle* 10 - bend radius* 11 - BOM elbow angle* 12 - BOM pipe length* 13 - BOM total pipe length* 14 - vertical axis* 15 - axis of rotation* 16 - clip axis* 17 - BOM route length* 18 - ignore BOM value

#### Return Value

String value for the specified aspect

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RoutingComponentManager::GetRoutingStringValue.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Routing Component Properties Example (C#)](Get_and_Set_Routing_Component_Properties_Example_CSharp.htm)

[Get and Set Routing Component Properties Example (VB.NET)](Get_and_Set_Routing_Component_Properties_Example_VBNET.htm)

[Get and Set Routing Component Properties Example (VBA)](Get_and_Set_Routing_Component_Properties_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingComponentManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager.html)

[IRoutingComponentManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRoutingComponentManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2011 FCS