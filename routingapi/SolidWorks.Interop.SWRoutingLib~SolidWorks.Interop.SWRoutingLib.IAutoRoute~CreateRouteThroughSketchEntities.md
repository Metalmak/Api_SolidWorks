<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute~CreateRouteThroughSketchEntities.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| CreateRouteThroughSketchEntities Method (IAutoRoute) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IAutoRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute.html) : CreateRouteThroughSketchEntities Method (IAutoRoute) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*conversionMode*
:   Type of route as defined in [swAutoRouteConversionMode\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swAutoRouteConversionMode_e.html)

*autoTangencyMode*
:   Tangency mode as defined in [swAutoRouteAutoTangencyMode\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swAutoRouteAutoTangencyMode_e.html)

*EntityTypes*
:   Array of the types of sketch entities to use for the route as defined in [swAutoRouteSketchEntitiesTypes\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swAutoRouteSketchEntitiesTypes_e.html) (see **Remarks**)

*EntityIDs*
:   Array of IDs of the sketch entities in EntityTypes (see **Remarks**)

Creates a route using the specified sketch entity types and IDs.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateRouteThroughSketchEntities( _    ByVal conversionMode As System.Integer, _    ByVal autoTangencyMode As System.Integer, _    ByVal EntityTypes As System.Object, _    ByVal EntityIDs As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAutoRoute Dim conversionMode As System.Integer Dim autoTangencyMode As System.Integer Dim EntityTypes As System.Object Dim EntityIDs As System.Object Dim value As System.Integer   value = instance.CreateRouteThroughSketchEntities(conversionMode, autoTangencyMode, EntityTypes, EntityIDs) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CreateRouteThroughSketchEntities(     System.int conversionMode,    System.int autoTangencyMode,    System.object EntityTypes,    System.object EntityIDs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CreateRouteThroughSketchEntities(  &   System.int conversionMode, &   System.int autoTangencyMode, &   System.Object^ EntityTypes, &   System.Object^ EntityIDs ) ``` | |

#### Parameters

*conversionMode*
:   Type of route as defined in [swAutoRouteConversionMode\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swAutoRouteConversionMode_e.html)

*autoTangencyMode*
:   Tangency mode as defined in [swAutoRouteAutoTangencyMode\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swAutoRouteAutoTangencyMode_e.html)

*EntityTypes*
:   Array of the types of sketch entities to use for the route as defined in [swAutoRouteSketchEntitiesTypes\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swAutoRouteSketchEntitiesTypes_e.html) (see **Remarks**)

*EntityIDs*
:   Array of IDs of the sketch entities in EntityTypes (see **Remarks**)

#### Return Value

Error code as defined in [swAutoRouteErrorType\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swAutoRouteErrorType_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AutoRoute::CreateRouteThroughSketchEntities.

# ![](dotnetimages/collapse.gif)Example

[Create Route Through Sketch Entities (C#)](Create_Route_Through_Sketch_Entities_Example_CSharp.htm)

[Create Route Through Sketch Entities (VB.NET)](Create_Route_Through_Sketch_Entities_Example_VBNET.htm)

[Create Route Through Sketch Entities (VBA)](Create_Route_Through_Sketch_Entities_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The EntityTypes and EntityIDs arrays must be the same size.

The EntityIDs determine the path of the route. To get EntityIDs values, use ISketchPoint::GetID for sketch points and ISketchSegment::GetID for sketch lines, sketch arcs, and sketch spline.

If a segment already exists between two sketch entities, then that segment is used as part of the newly created route path.

Before calling this method:

1. Select a route feature in an assembly.- Call [IRouteManager::EditRoute](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~EditRoute.html).- Populate the EntityTypes and EntityIDs arrays with the types and IDs of the sketch entities.

# ![](dotnetimages/collapse.gif)See Also

####

[IAutoRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute.html)

[IAutoRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute_members.html)

[IAutoRoute::ICreateRouteThroughSketchEntities Method ()](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute~ICreateRouteThroughSketchEntities.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2014 FCS