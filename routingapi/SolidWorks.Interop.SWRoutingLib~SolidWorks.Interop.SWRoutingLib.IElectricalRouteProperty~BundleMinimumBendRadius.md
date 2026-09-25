<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRouteProperty~BundleMinimumBendRadius.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| BundleMinimumBendRadius Property (IElectricalRouteProperty) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IElectricalRouteProperty Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRouteProperty.html) : BundleMinimumBendRadius Property (IElectricalRouteProperty) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the maximum bend radius of the individual wires in a bundle of wires that are routed through the same route segment.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property BundleMinimumBendRadius As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IElectricalRouteProperty Dim value As System.Double   value = instance.BundleMinimumBendRadius ``` | |

| C# |  |
| --- | --- |
| ``` System.double BundleMinimumBendRadius {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double BundleMinimumBendRadius {    System.double get(); } ``` | |

#### Property Value

Maximum bend radius of the individual wires in a bundle of wires that are routed through the same route segment

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ElectricalRouteProperty::BundleMinimumBendRadius.

# ![](dotnetimages/collapse.gif)Example

[Get Minimum Bend Radii of Wires (C#)](Get_Minimum_Bend_Radii_of_Wires_Example_CSharp.htm)

[Get Minimum Bend Radii of Wires (VB.NET)](Get_Minimum_Bend_Radii_of_Wires_Example_VBNET.htm)

[Get Minimum Bend Radii of Wires (VBA)](Get_Minimum_Bend_Radii_of_Wires_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The minimum bend radius for a bundle of wires routed through the same route segment is the maximum bend radius of the individual wires.

# ![](dotnetimages/collapse.gif)See Also

####

[IElectricalRouteProperty Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRouteProperty.html)

[IElectricalRouteProperty Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalRouteProperty_members.html)

[IRouteProperty::MinimumBendRadius Property ()](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteProperty~MinimumBendRadius.html)

[IRouteProperty::BendRadius Property ()](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteProperty~BendRadius.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2014 FCS