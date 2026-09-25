<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire~ISetRoutePathForWire.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| ISetRoutePathForWire Method (IWire) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IWire Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire.html) : ISetRoutePathForWire Method (IWire) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*numRouteSegmentIds*
:   Number of route segments in this wire

*RouteSegmentIDs*
:   * in-process, unmanaged C++: Pointer to an array of route segment IDs for this wire* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Sets a new route path for this wire.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ISetRoutePathForWire( _    ByVal numRouteSegmentIds As System.Integer, _    ByRef RouteSegmentIDs As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IWire Dim numRouteSegmentIds As System.Integer Dim RouteSegmentIDs As System.Integer Dim value As System.Integer   value = instance.ISetRoutePathForWire(numRouteSegmentIds, RouteSegmentIDs) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ISetRoutePathForWire(     System.int numRouteSegmentIds,    ref System.int RouteSegmentIDs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ISetRoutePathForWire(  &   System.int numRouteSegmentIds, &   System.int% RouteSegmentIDs ) ``` | |

#### Parameters

*numRouteSegmentIds*
:   Number of route segments in this wire

*RouteSegmentIDs*
:   * in-process, unmanaged C++: Pointer to an array of route segment IDs for this wire* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

#### Return Value

Status of setting a new route path as defined in [swSetRoutePathForWireErrorType\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swSetRoutePathForWireErrorType_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Wire::ISetRoutePathForWire.

# ![](dotnetimages/collapse.gif)Remarks

This method checks to see if the route segment IDs are valid. If so, then:

* the existing wire path is cleared.* a new wire path with new route segments is created.

You can pass new route segments by either:

* preselecting the route segments or preselecting two connectors. This method automatically detects the route segments between the two selected connectors.
  - or -* Passing an array of route segment IDs.

Before calling this method, call [IWire::GetRouteSegmentIDsCount](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IWire~GetRouteSegmentIDsCount.html) to get numRouteSegmentIDs.

# ![](dotnetimages/collapse.gif)See Also

####

[IWire Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire.html)

[IWire Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire_members.html)

[IWire::SetRoutePathForWire Method ()](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IWire~SetRoutePathForWire.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2014 FCS