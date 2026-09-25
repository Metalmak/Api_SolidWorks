<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute~IGetSketchSegments.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| IGetSketchSegments Method (IElectricalFlatRoute) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IElectricalFlatRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute.html) : IGetSketchSegments Method (IElectricalFlatRoute) |

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

*Count*
:   :   Number of SOLIDWORKS sketch segments

Gets all of the SOLIDWORKS sketch segments in the specified route segment for this flattened route.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetSketchSegments( _    ByVal RouteSegmentID As System.Integer, _    ByRef Count As System.Integer _ ) As System.IntPtr ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IElectricalFlatRoute Dim RouteSegmentID As System.Integer Dim Count As System.Integer Dim value As System.IntPtr   value = instance.IGetSketchSegments(RouteSegmentID, Count) ``` | |

| C# |  |
| --- | --- |
| ``` System.IntPtr IGetSketchSegments(     System.int RouteSegmentID,    out System.int Count ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.IntPtr IGetSketchSegments(  &   System.int RouteSegmentID, &   [Out] System.int Count ) ``` | |

#### Parameters

*RouteSegmentID*
:   :   Route segment ID (see Remarks)

*Count*
:   :   Number of SOLIDWORKS sketch segments

#### Return Value

* in-process, unmanaged C++: Pointer to an array of SOLIDWORKS sketch segments* VBA, VB.NET, C#, and C++/CLI: Not supported

See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Call [IWire::GetRouteSegmentIDs](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IWire~GetRouteSegmentIDs.html) to get the value for RouteSegmentID.

# ![](dotnetimages/collapse.gif)See Also

####

[IElectricalFlatRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute.html)

[IElectricalFlatRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute_members.html)

[IElectricalFlatRoute::GetSketchSegments Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute~GetSketchSegments.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2009 FCS