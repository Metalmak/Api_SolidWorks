<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute~ConvertGuidelinesToRoute.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| ConvertGuidelinesToRoute Method (IAutoRoute) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IAutoRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute.html) : ConvertGuidelinesToRoute Method (IAutoRoute) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Converts selected guidelines into unique routes.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ConvertGuidelinesToRoute() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAutoRoute Dim value As System.Boolean   value = instance.ConvertGuidelinesToRoute() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ConvertGuidelinesToRoute() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ConvertGuidelinesToRoute(); ``` | |

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AutoRoute::ConvertGuidelinesToRoute.

# ![](dotnetimages/collapse.gif)Example

[Convert Guidelines into a Route Example (C#)](Convert_Guidelines_into_a_Route_Example_CSharp.htm)

[Convert Guidelines into a Route Example (VB.NET)](Convert_Guidelines_into_a_Route_Example_VBNET.htm)

[Convert Guidelines into a Route Example (VBA)](Convert_Guidelines_into_a_Route_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method:

1. Call [IRouteManager::ImportFromToList](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~ImportFromToList.html).- In the FeatureManager design tree, select the assembly that contains the route whose guidelines you want to select.- Call [IRouteManager::EditRoute](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~EditRoute.html).- Call IModelDocExtension::SelectByID2 multiple times specifying type SKETCHSEGMENT to mark the guidelines you want to convert or call [IAutoRoute::SelectGuidelines](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IAutoRoute~SelectGuidelines.html) to select all guidelines.

# ![](dotnetimages/collapse.gif)See Also

####

[IAutoRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute.html)

[IAutoRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2011 FCS