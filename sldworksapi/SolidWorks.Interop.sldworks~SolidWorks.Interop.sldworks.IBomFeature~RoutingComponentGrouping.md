<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~RoutingComponentGrouping.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RoutingComponentGrouping Property (IBomFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature.html) : RoutingComponentGrouping Property (IBomFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the routing component grouping options for this BOM table in a drawing of an assembly containing routing components.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property RoutingComponentGrouping As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomFeature Dim value As System.Integer   instance.RoutingComponentGrouping = value   value = instance.RoutingComponentGrouping ``` | |

| C# |  |
| --- | --- |
| ``` System.int RoutingComponentGrouping {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int RoutingComponentGrouping {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Routing component grouping options as defined in swRoutingComponentGroupOption\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BomFeature::RoutingComponentGrouping.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Routing Component Grouping Options for BOM Table (C#)](Get_and_Set_Routing_Component_Grouping_Options_for_BOM_Table_Example_CSharp.htm)

[Get and Set Routing Component Grouping Options for BOM Table (VB.NET)](Get_and_Set_Routing_Component_Grouping_Options_for_BOM_Table_Example_VBNET.htm)

[Get and Set Routing Component Grouping Options for BOM Table (VBA)](Get_and_Set_Routing_Component_Grouping_Options_for_BOM_Table_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IBomFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature.html)

[IBomFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0