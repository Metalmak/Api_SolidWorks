<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute~GetConnectorData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetConnectorData Method (IElectricalFlatRoute) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IElectricalFlatRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute.html) : GetConnectorData Method (IElectricalFlatRoute) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*connectorName*
:   Name of the connector

*fittingPoint*
:   Location of the fitting's connection point in the flattened configuration

*fittingDirection*
:   Array of doubles for the direction in which the route exits the fitting at the connection point in the flattened configuration

*isVisible*
:   TRUE if the connector is visible, FALSE if not

Gets the specified connector's data for this electrical flattened route.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetConnectorData( _    ByVal connectorName As System.String, _    ByRef fittingPoint As System.Object, _    ByRef fittingDirection As System.Object, _    ByRef isVisible As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IElectricalFlatRoute Dim connectorName As System.String Dim fittingPoint As System.Object Dim fittingDirection As System.Object Dim isVisible As System.Boolean Dim value As System.Boolean   value = instance.GetConnectorData(connectorName, fittingPoint, fittingDirection, isVisible) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetConnectorData(     System.string connectorName,    out System.object fittingPoint,    out System.object fittingDirection,    out System.bool isVisible ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetConnectorData(  &   System.String^ connectorName, &   [Out] System.Object^ fittingPoint, &   [Out] System.Object^ fittingDirection, &   [Out] System.bool isVisible ) ``` | |

#### Parameters

*connectorName*
:   Name of the connector

*fittingPoint*
:   Location of the fitting's connection point in the flattened configuration

*fittingDirection*
:   Array of doubles for the direction in which the route exits the fitting at the connection point in the flattened configuration

*isVisible*
:   TRUE if the connector is visible, FALSE if not

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ElectricalFlatRoute::GetConnectorData.

# ![](dotnetimages/collapse.gif)See Also

####

[IElectricalFlatRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute.html)

[IElectricalFlatRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute_members.html)

[IElectricalFlatRoute::IGetConnectorData Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute~IGetConnectorData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2008 FCS