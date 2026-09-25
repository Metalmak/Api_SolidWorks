<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~CreatePipeDrawingforPipeRoute.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| CreatePipeDrawingforPipeRoute Method (IRouteManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html) : CreatePipeDrawingforPipeRoute Method (IRouteManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BOMTemplatePath*
:   Fully specified path of the BOM template; only valid if insertBOM = true

*BOMTemplateName*
:   Name of the BOM template; only valid if insertBOM = true

*insertBalloons*
:   True to include auto balloons in the drawing, false to not

*insertBOM*
:   True to include a BOM table, false to not

*showSketch*
:   True to include the route sketch in the drawing; false to not

*subAssembly*
:   True to include dimensions of sub-assemblies in the drawing, false to not

*userSheetWidth*
:   Width of custom sheet; specify 0.0 if standard sheet is specified in dwgTemplates

*userSheetHeight*
:   Height of custom sheet; specify 0.0 if standard sheet is specified in dwgTemplates

*sheetTemplatePath*
:   Fully specified path of drawing sheet templates

*sheetTemplateName*
:   Name of drawing sheet template

*displayFormat*
:   True to display the sheet format in the drawing, false to not

*dwgTemplates*
:   SOLIDWORKS drawing sheet template as defined in swDwgTemplates\_e

Creates a drawing of a piping assembly that includes fittings, pipes, dimensions, and a BOM in an isometric view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub CreatePipeDrawingforPipeRoute( _    ByVal BOMTemplatePath As System.String, _    ByVal BOMTemplateName As System.String, _    ByVal insertBalloons As System.Boolean, _    ByVal insertBOM As System.Boolean, _    ByVal showSketch As System.Boolean, _    ByVal subAssembly As System.Boolean, _    ByVal userSheetWidth As System.Double, _    ByVal userSheetHeight As System.Double, _    ByVal sheetTemplatePath As System.String, _    ByVal sheetTemplateName As System.String, _    ByVal displayFormat As System.Boolean, _    ByVal dwgTemplates As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRouteManager Dim BOMTemplatePath As System.String Dim BOMTemplateName As System.String Dim insertBalloons As System.Boolean Dim insertBOM As System.Boolean Dim showSketch As System.Boolean Dim subAssembly As System.Boolean Dim userSheetWidth As System.Double Dim userSheetHeight As System.Double Dim sheetTemplatePath As System.String Dim sheetTemplateName As System.String Dim displayFormat As System.Boolean Dim dwgTemplates As System.Integer   instance.CreatePipeDrawingforPipeRoute(BOMTemplatePath, BOMTemplateName, insertBalloons, insertBOM, showSketch, subAssembly, userSheetWidth, userSheetHeight, sheetTemplatePath, sheetTemplateName, displayFormat, dwgTemplates) ``` | |

| C# |  |
| --- | --- |
| ``` void CreatePipeDrawingforPipeRoute(     System.string BOMTemplatePath,    System.string BOMTemplateName,    System.bool insertBalloons,    System.bool insertBOM,    System.bool showSketch,    System.bool subAssembly,    System.double userSheetWidth,    System.double userSheetHeight,    System.string sheetTemplatePath,    System.string sheetTemplateName,    System.bool displayFormat,    System.int dwgTemplates ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CreatePipeDrawingforPipeRoute(  &   System.String^ BOMTemplatePath, &   System.String^ BOMTemplateName, &   System.bool insertBalloons, &   System.bool insertBOM, &   System.bool showSketch, &   System.bool subAssembly, &   System.double userSheetWidth, &   System.double userSheetHeight, &   System.String^ sheetTemplatePath, &   System.String^ sheetTemplateName, &   System.bool displayFormat, &   System.int dwgTemplates ) ``` | |

#### Parameters

*BOMTemplatePath*
:   Fully specified path of the BOM template; only valid if insertBOM = true

*BOMTemplateName*
:   Name of the BOM template; only valid if insertBOM = true

*insertBalloons*
:   True to include auto balloons in the drawing, false to not

*insertBOM*
:   True to include a BOM table, false to not

*showSketch*
:   True to include the route sketch in the drawing; false to not

*subAssembly*
:   True to include dimensions of sub-assemblies in the drawing, false to not

*userSheetWidth*
:   Width of custom sheet; specify 0.0 if standard sheet is specified in dwgTemplates

*userSheetHeight*
:   Height of custom sheet; specify 0.0 if standard sheet is specified in dwgTemplates

*sheetTemplatePath*
:   Fully specified path of drawing sheet templates

*sheetTemplateName*
:   Name of drawing sheet template

*displayFormat*
:   True to display the sheet format in the drawing, false to not

*dwgTemplates*
:   SOLIDWORKS drawing sheet template as defined in swDwgTemplates\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RouteManager::CreatePipeDrawingforPipeRoute.

# ![](dotnetimages/collapse.gif)Example

[Create a Drawing for a Pipe Route Example (VBA)](Create_a_Drawing_for_a_Pipe_Route_Example_VB.htm)

[Create a Drawing for a Pipe Route Example (VB.NET)](Create_a_Drawing_for_a_Pipe_Route_Example_VBNET.htm)

[Create a Drawing for a Pipe Route Example (C#)](Create_a_Drawing_for_a_Pipe_Route_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html)

[IRouteManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2011 FCS