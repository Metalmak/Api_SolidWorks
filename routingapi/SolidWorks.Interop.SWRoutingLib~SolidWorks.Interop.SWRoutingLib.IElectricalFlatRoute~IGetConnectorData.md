<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute~IGetConnectorData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| IGetConnectorData Method (IElectricalFlatRoute) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IElectricalFlatRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute.html) : IGetConnectorData Method (IElectricalFlatRoute) |

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
:   * in-process, unmanaged C++: Pointer to an array of doubles for the direction in which the route exits the fitting at the connection point in the flattened configuration* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*isVisible*
:   True if the connector is visible, false if not

Gets the specified connector's data for this electrical flattened route.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetConnectorData( _    ByVal connectorName As System.String, _    ByRef fittingPoint As System.Object, _    ByRef fittingDirection As System.Double, _    ByRef isVisible As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IElectricalFlatRoute Dim connectorName As System.String Dim fittingPoint As System.Object Dim fittingDirection As System.Double Dim isVisible As System.Boolean Dim value As System.Boolean   value = instance.IGetConnectorData(connectorName, fittingPoint, fittingDirection, isVisible) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IGetConnectorData(     System.string connectorName,    out System.object fittingPoint,    out System.double fittingDirection,    out System.bool isVisible ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IGetConnectorData(  &   System.String^ connectorName, &   [Out] System.Object^ fittingPoint, &   [Out] System.double fittingDirection, &   [Out] System.bool isVisible ) ``` | |

#### Parameters

*connectorName*
:   Name of the connector

*fittingPoint*
:   Location of the fitting's connection point in the flattened configuration

*fittingDirection*
:   * in-process, unmanaged C++: Pointer to an array of doubles for the direction in which the route exits the fitting at the connection point in the flattened configuration* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*isVisible*
:   True if the connector is visible, false if not

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)See Also

####

[IElectricalFlatRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute.html)

[IElectricalFlatRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute_members.html)

[IElectricalFlatRoute::GetConnectorData Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute~GetConnectorData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2008 FCS