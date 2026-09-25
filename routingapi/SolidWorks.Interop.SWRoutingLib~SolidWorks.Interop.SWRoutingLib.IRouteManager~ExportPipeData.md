<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~ExportPipeData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| ExportPipeData Method (IRouteManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html) : ExportPipeData Method (IRouteManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*fileName*
:   Directory path where *<piping\_assembly\_name>.*pcf is created

*units*
:   Units of exported pipe data

    * 0 = millimeters* 3 = inches

*options*
:   Export options; not yet defined

Exports pipe data in Piping Component File (PCF) format.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ExportPipeData( _    ByVal fileName As System.String, _    ByVal units As System.Integer, _    ByVal options As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRouteManager Dim fileName As System.String Dim units As System.Integer Dim options As System.Integer Dim value As System.Integer   value = instance.ExportPipeData(fileName, units, options) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ExportPipeData(     System.string fileName,    System.int units,    System.int options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ExportPipeData(  &   System.String^ fileName, &   System.int units, &   System.int options ) ``` | |

#### Parameters

*fileName*
:   Directory path where *<piping\_assembly\_name>.*pcf is created

*units*
:   Units of exported pipe data

    * 0 = millimeters* 3 = inches

*options*
:   Export options; not yet defined

#### Return Value

Status as defined in [swRoutingExportPipeDataError\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swRoutingExportPipeDataError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RouteManager::ExportPipeData.

# ![](dotnetimages/collapse.gif)Example

[Export Pipe Data Example (C#)](Export_Pipe_Data_Example_CSharp.htm)

[Export Pipe Data Example (VB.NET)](Export_Pipe_Data_Example_VBNET.htm)

[Export Pipe Data Example (VBA)](Export_Pipe_Data_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is only valid for use with assemblies containing pipes.

# ![](dotnetimages/collapse.gif)See Also

####

[IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html)

[IRouteManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2008 FCS