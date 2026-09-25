<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute~GetRouteSegmentID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetRouteSegmentID Method (IElectricalRoute) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IElectricalRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute.html) : GetRouteSegmentID Method (IElectricalRoute) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SketchSegment*
:   SOLIDWORKS sketch segment

Gets the route segment ID for the specified SOLIDWORKS sketch segment.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetRouteSegmentID( _    ByVal SketchSegment As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IElectricalRoute Dim SketchSegment As System.Object Dim value As System.Integer   value = instance.GetRouteSegmentID(SketchSegment) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetRouteSegmentID(     System.object SketchSegment ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetRouteSegmentID(  &   System.Object^ SketchSegment ) ``` | |

#### Parameters

*SketchSegment*
:   SOLIDWORKS sketch segment

#### Return Value

Route segment ID

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ElectricalRoute::GetRouteSegmentID.

# ![](dotnetimages/collapse.gif)Remarks

If the sketch segment is not a route, then RouteSegmentID is set to -1.

Use [IElectricalRoute::GetSketchSegments](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IElectricalRoute~GetSketchSegments.html) or [IElectricalRoute::IGetSketchSegments](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IElectricalRoute~IGetSketchSegments.html) to get the SOLIDWORKS sketch segments.

# ![](dotnetimages/collapse.gif)See Also

####

[IElectricalRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute.html)

[IElectricalRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute_members.html)

[IElectricalRoute::GetRouteProperty Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute~GetRouteProperty.html)

[IElectricalRoute::GetSketchSegmentsCount Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute~GetSketchSegmentsCount.html)

[IWire::GetRouteSegmentIDs Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire~GetRouteSegmentIDs.html)

[IWire::IGetRouteSegmentIDs Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire~IGetRouteSegmentIDs.html)

[IWire::GetRouteSegmentIDsCount Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire~GetRouteSegmentIDsCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2006 FCS