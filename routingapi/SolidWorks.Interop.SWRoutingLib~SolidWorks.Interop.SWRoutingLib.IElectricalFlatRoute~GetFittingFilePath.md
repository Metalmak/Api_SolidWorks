<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute~GetFittingFilePath.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetFittingFilePath Method (IElectricalFlatRoute) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IElectricalFlatRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute.html) : GetFittingFilePath Method (IElectricalFlatRoute) |

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

Gets the path and filename of the fitting for the specified connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFittingFilePath( _    ByVal connectorName As System.String _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IElectricalFlatRoute Dim connectorName As System.String Dim value As System.String   value = instance.GetFittingFilePath(connectorName) ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetFittingFilePath(     System.string connectorName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetFittingFilePath(  &   System.String^ connectorName ) ``` | |

#### Parameters

*connectorName*
:   Name of the connector

#### Return Value

Path and filename of the fitting

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ElectricalFlatRoute::GetFittingFilePath.

# ![](dotnetimages/collapse.gif)See Also

####

[IElectricalFlatRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute.html)

[IElectricalFlatRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2008 FCS