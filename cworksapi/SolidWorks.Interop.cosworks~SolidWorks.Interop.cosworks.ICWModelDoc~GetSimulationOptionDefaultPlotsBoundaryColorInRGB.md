<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~GetSimulationOptionDefaultPlotsBoundaryColorInRGB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetSimulationOptionDefaultPlotsBoundaryColorInRGB Method (ICWModelDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) : GetSimulationOptionDefaultPlotsBoundaryColorInRGB Method (ICWModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NBoundaryOption*
:   Boundary option as defined in [swsSimulationOptionDefaultPlotsBoundaryColorInRGBBoundaryOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSimulationOptionDefaultPlotsBoundaryColorInRGBBoundaryOption_e.html)

*ErrorCode*
:   Error code as defined in [swsSimulationOptionDefaultPlotsBoundaryColorInRGBError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsSimulationOptionDefaultPlotsBoundaryColorInRGBError_e.html)

Gets the RGB color for the specified default plot boundary option.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSimulationOptionDefaultPlotsBoundaryColorInRGB( _    ByVal NBoundaryOption As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWModelDoc Dim NBoundaryOption As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetSimulationOptionDefaultPlotsBoundaryColorInRGB(NBoundaryOption, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetSimulationOptionDefaultPlotsBoundaryColorInRGB(     System.int NBoundaryOption,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetSimulationOptionDefaultPlotsBoundaryColorInRGB(  &   System.int NBoundaryOption, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NBoundaryOption*
:   Boundary option as defined in [swsSimulationOptionDefaultPlotsBoundaryColorInRGBBoundaryOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSimulationOptionDefaultPlotsBoundaryColorInRGBBoundaryOption_e.html)

*ErrorCode*
:   Error code as defined in [swsSimulationOptionDefaultPlotsBoundaryColorInRGBError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsSimulationOptionDefaultPlotsBoundaryColorInRGBError_e.html)

#### Return Value

Array of three values; [0-255][0-255][0-255]

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWModelDoc::GetSimulationOptionDefaultPlotsBoundaryColorInRGB.

# ![](dotnetimages/collapse.gif)Example

[Analyze Part (VBA)](Analyze_Part_Example_VB.htm)

[Analyze Part (VB.NET)](Analyze_Part_Example_VBNET.htm)

[Analyze Part (C#)](Analyze_Part_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html)

[ICWModelDoc Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc_members.html)

[ICWModelDoc::SetSimulationOptionDefaultPlotsBoundaryColorInRGB Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~SetSimulationOptionDefaultPlotsBoundaryColorInRGB.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0