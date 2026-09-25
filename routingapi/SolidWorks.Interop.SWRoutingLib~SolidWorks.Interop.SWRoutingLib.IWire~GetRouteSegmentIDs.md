<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire~GetRouteSegmentIDs.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetRouteSegmentIDs Method (IWire) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IWire Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire.html) : GetRouteSegmentIDs Method (IWire) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the route segment IDs in this wire.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetRouteSegmentIDs() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IWire Dim value As System.Object   value = instance.GetRouteSegmentIDs() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetRouteSegmentIDs() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetRouteSegmentIDs(); ``` | |

#### Return Value

Array of route segment IDs

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Wire::GetRouteSegmentIDs.

# ![](dotnetimages/collapse.gif)Example

[Get Wires, Sketch Segments, and Sketches (VBA)](Get_Wires_Sketch_Segments_and_Sketches_Example_VB.htm)

[Set New Route Paths for Wires (C#)](Set_New_Route_Paths_for_Wires_Example_CSharp.htm)

[Set New Route Paths for Wires (VB.NET)](Set_New_Route_Paths_for_Wires_Example_VBNET.htm)

[Set New Route Paths for Wires (VBA)](Set_New_Route_Paths_for_Wires_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IWire Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire.html)

[IWire Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire_members.html)

[IWire::IGetRouteSegmentIDs Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire~IGetRouteSegmentIDs.html)

[IWire::GetRouteSegmentIDsCount Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire~GetRouteSegmentIDsCount.html)

[IElectricalRoute::GetRouteProperty Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute~GetRouteProperty.html)

[IElectricalRoute::GetRouteSegmentID Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute~GetRouteSegmentID.html)

[IElectricalRoute::GetSketchSegments Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute~GetSketchSegments.html)

[IElectricalRoute::GetSketchSegmentsCount Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute~GetSketchSegmentsCount.html)

[IElectricalRoute::IGetSketchSegments Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRoute~IGetSketchSegments.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2006 FCS