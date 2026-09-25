<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute~GetSketchSegmentsCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetSketchSegmentsCount Method (IElectricalRoute) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IElectricalRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute.html) : GetSketchSegmentsCount Method (IElectricalRoute) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RouteSegmentID*
:   Route segment ID (see Remarks)

Gets the number of SOLIDWORKS sketch segments in the route segment using the specified route segment ID.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSketchSegmentsCount( _    ByVal RouteSegmentID As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IElectricalRoute Dim RouteSegmentID As System.Integer Dim value As System.Integer   value = instance.GetSketchSegmentsCount(RouteSegmentID) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetSketchSegmentsCount(     System.int RouteSegmentID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetSketchSegmentsCount(  &   System.int RouteSegmentID ) ``` | |

#### Parameters

*RouteSegmentID*
:   Route segment ID (see Remarks)

#### Return Value

Number of sketch segments

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ElectricalRoute::GetSketchSegmentsCount.

# ![](dotnetimages/collapse.gif)Remarks

Use [IWire::GetRouteSegmentIDs](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IWire~GetRouteSegmentIDs.html) to get the value for RouteSegmentID.

Call this method before calling [IElectricalRoute::IGetSketchSegments](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IElectricalRoute~IGetSketchSegments.html) to determine the size of the array for the sketch segments.

# ![](dotnetimages/collapse.gif)See Also

####

[IElectricalRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute.html)

[IElectricalRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute_members.html)

[IElectricalRoute::GetSketchSegments Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute~GetSketchSegments.html)

[IElectricalRoute::GetRouteProperty Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute~GetRouteProperty.html)

[IElectricalRoute::GetRouteSegmentID Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute~GetRouteSegmentID.html)

[IWire::GetRouteSegmentIDs Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire~GetRouteSegmentIDs.html)

[IWire::IGetRouteSegmentIDs Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire~IGetRouteSegmentIDs.html)

[IWire::GetRouteSegmentIDsCount Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire~GetRouteSegmentIDsCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2006 FCS