<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~ExportTubeData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| ExportTubeData Method (IRouteManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html) : ExportTubeData Method (IRouteManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*fileName*
:   Specify *<path\_name>.<file\_extension>*; for example, specify **c:\temp.html** to create **default.html** in **c:\temp**

*type*
:   Bend data type as defined in [swExportTubeDataReportType\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swExportTubeDataReportType_e.html)

*options*
:   Export options; not yet defined

Exports an HTML bend data table containing the tangent or intersection points in a tubing assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ExportTubeData( _    ByVal fileName As System.String, _    ByVal type As System.Integer, _    ByVal options As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRouteManager Dim fileName As System.String Dim type As System.Integer Dim options As System.Integer Dim value As System.Integer   value = instance.ExportTubeData(fileName, type, options) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ExportTubeData(     System.string fileName,    System.int type,    System.int options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ExportTubeData(  &   System.String^ fileName, &   System.int type, &   System.int options ) ``` | |

#### Parameters

*fileName*
:   Specify *<path\_name>.<file\_extension>*; for example, specify **c:\temp.html** to create **default.html** in **c:\temp**

*type*
:   Bend data type as defined in [swExportTubeDataReportType\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swExportTubeDataReportType_e.html)

*options*
:   Export options; not yet defined

#### Return Value

Status as defined in [swRoutingExportDataError\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swRoutingExportDataError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RouteManager::ExportTubeData.

# ![](dotnetimages/collapse.gif)Example

[Export Tube Data Example (C#)](Export_Tube_Data_Example_CSharp.htm)

[Export Tube Data Example (VB.NET)](Export_Tube_Data_Example_VBNET.htm)

[Export Tube Data Example (VBA)](Export_Tube_Data_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is only valid for use with assemblies containing tubes.

# ![](dotnetimages/collapse.gif)See Also

####

[IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html)

[IRouteManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2011 FCS