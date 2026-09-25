<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute~CreatePointToPointAutoRoute.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| CreatePointToPointAutoRoute Method (IAutoRoute) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IAutoRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute.html) : CreatePointToPointAutoRoute Method (IAutoRoute) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*conversionMode*
:   Route style as defined in [swPointToPointAutoRouteConversionMode\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swPointToPointAutoRouteConversionMode_e.html)

Connects two selected entities on a route.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreatePointToPointAutoRoute( _    ByVal conversionMode As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAutoRoute Dim conversionMode As System.Integer Dim value As System.Integer   value = instance.CreatePointToPointAutoRoute(conversionMode) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CreatePointToPointAutoRoute(     System.int conversionMode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CreatePointToPointAutoRoute(  &   System.int conversionMode ) ``` | |

#### Parameters

*conversionMode*
:   Route style as defined in [swPointToPointAutoRouteConversionMode\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swPointToPointAutoRouteConversionMode_e.html)

#### Return Value

Error code as defined in [swPointToPointAutoRouteErrorType\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swPointToPointAutoRouteErrorType_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AutoRoute::CreatePointToPointAutoRoute.

# ![](dotnetimages/collapse.gif)Example

[Create Auto Route Example (C#)](Create_Auto_Route_Example_CSharp.htm)

[Create Auto Route Example (VB.NET)](Create_Auto_Route_Example_VBNET.htm)

[Create Auto Route Example (VBA)](Create_Auto_Route_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call this method to automatically connect one of the following in a route:

* two points* a point and a clip axis* a point and a line

Before calling this method:

1. In the FeatureManager design tree, select the assembly that contains the route to which to add connections.- Call [IRouteManager::EditRoute](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~EditRoute.html).- Call IModelDocExtension::SelectByID2 twice, specifying type SKETCHPOINT to select two points on the route.

After calling this method:

1. Call [IRouteManager::ExitRoute](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~ExitRoute.html).- Call IAssemblyDoc::EditAssembly.

# ![](dotnetimages/collapse.gif)See Also

####

[IAutoRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute.html)

[IAutoRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2011 FCS