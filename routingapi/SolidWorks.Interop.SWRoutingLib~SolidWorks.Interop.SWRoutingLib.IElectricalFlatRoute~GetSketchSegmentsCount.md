<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute~GetSketchSegmentsCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetSketchSegmentsCount Method (IElectricalFlatRoute) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IElectricalFlatRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute.html) : GetSketchSegmentsCount Method (IElectricalFlatRoute) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RouteSegmentID*
:   :   Route segment ID (see Remarks)

Gets the number of SOLIDWORKS sketch segments for the specified route segment in this flattened route.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSketchSegmentsCount( _    ByVal RouteSegmentID As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IElectricalFlatRoute Dim RouteSegmentID As System.Integer Dim value As System.Integer   value = instance.GetSketchSegmentsCount(RouteSegmentID) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetSketchSegmentsCount(     System.int RouteSegmentID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetSketchSegmentsCount(  &   System.int RouteSegmentID ) ``` | |

#### Parameters

*RouteSegmentID*
:   :   Route segment ID (see Remarks)

#### Return Value

Number of segment segments

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ElectricalFlatRoute::GetSketchSegmentsCount.

# ![](dotnetimages/collapse.gif)Remarks

Use [IWire::GetRouteSegmentIDs](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IWire~GetRouteSegmentIDs.html) to get the value for RouteSegmentID.

Call this method before calling [IElectricalFlatRoute::IGetSketchSegments](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IElectricalFlatRoute~IGetSketchSegments.html) to determine the size of the array for the sketch segments.

# ![](dotnetimages/collapse.gif)See Also

####

[IElectricalFlatRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute.html)

[IElectricalFlatRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute_members.html)

[IElectricalFlatRoute::GetSketchSegments Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute~GetSketchSegments.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2009 FCS