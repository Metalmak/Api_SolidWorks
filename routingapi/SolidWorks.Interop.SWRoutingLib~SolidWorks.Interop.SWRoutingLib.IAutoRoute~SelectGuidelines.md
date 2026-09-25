<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute~SelectGuidelines.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| SelectGuidelines Method (IAutoRoute) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IAutoRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute.html) : SelectGuidelines Method (IAutoRoute) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Selects all of the guidelines in the route.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SelectGuidelines() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAutoRoute Dim value As System.Integer   value = instance.SelectGuidelines() ``` | |

| C# |  |
| --- | --- |
| ``` System.int SelectGuidelines() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SelectGuidelines(); ``` | |

#### Return Value

Number of selected guidelines

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AutoRoute::SelectGuidelines.

# ![](dotnetimages/collapse.gif)Example

[Merge Guidelines into a Route Example (C#)](Merge_Guidelines_into_a_Route_Example_CSharp.htm)

[Merge Guidelines into a Route Example (VB.NET)](Merge_Guidelines_into_a_Route_Example_VBNET.htm)

[Merge Guidelines into a Route Example (VBA)](Merge_Guidelines_into_a_Route_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method:

1. Call [IRouteManager::ImportFromToList](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~ImportFromToList.html).- In the FeatureManager design tree, select the assembly that contains the route whose guidelines to select.- Call [IRouteManager::EditRoute](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~EditRoute.html).

After calling this method, you can call:

* [IAutoRoute::MergeGuidelines](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IAutoRoute~MergeGuidelines.html)
  - or -* [IAutoRoute::ConvertGuidelinesToRoute](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IAutoRoute~ConvertGuidelinesToRoute.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IAutoRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute.html)

[IAutoRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute_members.html)

[IAutoRoute::DeleteAllGuidelines Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute~DeleteAllGuidelines.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2011 FCS