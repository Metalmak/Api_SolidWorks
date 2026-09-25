<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute~ShowGuidelines.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| ShowGuidelines Method (IAutoRoute) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IAutoRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute.html) : ShowGuidelines Method (IAutoRoute) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Displays a preview of the connections imported from a from-to list.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ShowGuidelines() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAutoRoute Dim value As System.Integer   value = instance.ShowGuidelines() ``` | |

| C# |  |
| --- | --- |
| ``` System.int ShowGuidelines() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ShowGuidelines(); ``` | |

#### Return Value

Number of displayed guidelines.

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AutoRoute::ShowGuidelines.

# ![](dotnetimages/collapse.gif)Example

[Merge Guidelines into a Route Example (C#)](Merge_Guidelines_into_a_Route_Example_CSharp.htm)

[Merge Guidelines into a Route Example (VB.NET)](Merge_Guidelines_into_a_Route_Example_VBNET.htm)

[Merge Guidelines into a Route Example (VBA)](Merge_Guidelines_into_a_Route_Example_VB.htm)

[Convert Guidelines into a Route Example (C#)](Convert_Guidelines_into_a_Route_Example_CSharp.htm)

[Convert Guidelines into a Route Example (VB.NET)](Convert_Guidelines_into_a_Route_Example_VBNET.htm)

[Convert Guidelines into a Route Example (VBA)](Convert_Guidelines_into_a_Route_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method:

1. Call [IRouteManager::ImportFromToList](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~ImportFromToList.html).- In the FeatureManager design tree, select the assembly that contains the route for which to show guidelines.- Call [IRouteManager::EditRoute](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~EditRoute.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IAutoRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute.html)

[IAutoRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2011 FCS