<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~SetSimulationOptionDefaultPlotsBoundaryColorInRGB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetSimulationOptionDefaultPlotsBoundaryColorInRGB Method (ICWModelDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) : SetSimulationOptionDefaultPlotsBoundaryColorInRGB Method (ICWModelDoc) |

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

*NRed*
:   0 <= Red component <= 255

*NGreen*
:   0 <= Green component <= 255

*NBlue*
:   0 <= Blue component <= 255

Sets the RGB color for the specified default plot boundary option.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSimulationOptionDefaultPlotsBoundaryColorInRGB( _    ByVal NBoundaryOption As System.Integer, _    ByVal NRed As System.Integer, _    ByVal NGreen As System.Integer, _    ByVal NBlue As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWModelDoc Dim NBoundaryOption As System.Integer Dim NRed As System.Integer Dim NGreen As System.Integer Dim NBlue As System.Integer Dim value As System.Integer   value = instance.SetSimulationOptionDefaultPlotsBoundaryColorInRGB(NBoundaryOption, NRed, NGreen, NBlue) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetSimulationOptionDefaultPlotsBoundaryColorInRGB(     System.int NBoundaryOption,    System.int NRed,    System.int NGreen,    System.int NBlue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetSimulationOptionDefaultPlotsBoundaryColorInRGB(  &   System.int NBoundaryOption, &   System.int NRed, &   System.int NGreen, &   System.int NBlue ) ``` | |

#### Parameters

*NBoundaryOption*
:   Boundary option as defined in [swsSimulationOptionDefaultPlotsBoundaryColorInRGBBoundaryOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSimulationOptionDefaultPlotsBoundaryColorInRGBBoundaryOption_e.html)

*NRed*
:   0 <= Red component <= 255

*NGreen*
:   0 <= Green component <= 255

*NBlue*
:   0 <= Blue component <= 255

#### Return Value

Error code as defined in [swsSimulationOptionDefaultPlotsBoundaryColorInRGBError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsSimulationOptionDefaultPlotsBoundaryColorInRGBError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWModelDoc::SetSimulationOptionDefaultPlotsBoundaryColorInRGB.

# ![](dotnetimages/collapse.gif)Example

[Analyze Part (VBA)](Analyze_Part_Example_VB.htm)

[Analyze Part (VB.NET)](Analyze_Part_Example_VBNET.htm)

[Analyze Part (C#)](Analyze_Part_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html)

[ICWModelDoc Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc_members.html)

[ICWModelDoc::GetSimulationOptionDefaultPlotsBoundaryColorInRGB Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~GetSimulationOptionDefaultPlotsBoundaryColorInRGB.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0