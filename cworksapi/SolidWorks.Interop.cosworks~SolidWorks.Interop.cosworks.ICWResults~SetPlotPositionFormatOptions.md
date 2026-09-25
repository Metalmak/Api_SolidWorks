<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotPositionFormatOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetPlotPositionFormatOptions Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : SetPlotPositionFormatOptions Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SPlotName*
:   Plot name (see **Remarks**)

*ArrayInput*
:   Array of position/format options (see **Remarks**)

Sets the position/format options for the specified plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPlotPositionFormatOptions( _    ByVal SPlotName As System.String, _    ByVal ArrayInput As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim SPlotName As System.String Dim ArrayInput As System.Object Dim value As System.Integer   value = instance.SetPlotPositionFormatOptions(SPlotName, ArrayInput) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetPlotPositionFormatOptions(     System.string SPlotName,    System.object ArrayInput ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetPlotPositionFormatOptions(  &   System.String^ SPlotName, &   System.Object^ ArrayInput ) ``` | |

#### Parameters

*SPlotName*
:   Plot name (see **Remarks**)

*ArrayInput*
:   Array of position/format options (see **Remarks**)

#### Return Value

Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::SetPlotPositionFormatOptions.

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWResults::GetPlotNames](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotNames.html) to populate SPlotName.

The 0-based array contains eight elements:

| Array element... | Contains... |
| --- | --- |
| 0 | Double[0,1]; horizontal position from the left of the graphics area; percentage of the window width |
| 1 | Double[0,1]; vertical position from the top of the graphics area; percentage of the window height |
| 2 | Chart width option as defined in [swsColorChartWidthOptionValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsColorChartWidthOptionValue_e.html) |
| 3 | Chart number format as defined in [swsColorChartNumberFormatOptionValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsColorChartNumberFormatOptionValue_e.html) |
| 4 | 0 <= Number of decimal places to display <= 16 |
| 5 | Boolean; whether to display chart numbers with a 1000 comma separator; valid only if array element 3 is swsColorChartNumberFormatOptionValue\_e.swsColorChartNumberFormatFloating or swsColorChartNumberFormatOptionValue\_e.swsColorChartNumberFormatGeneral |
| 6 | Boolean; whether to use different number format for small numbers (0.001 < |x| < 1000); valid only if array element 3 is swsColorChartNumberFormatOptionValue\_e.swsColorChartNumberFormatScientific |
| 7 | Number format for small numbers as defined in [swsColorNumberFormatUseDiffNumberFormatOptionValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsColorNumberFormatUseDiffNumberFormatOptionValue_e.html); valid only if array element 6 is true |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetPlotPositionFormatOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotPositionFormatOptions.html)

[ICWResults::SetPlotColorOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotColorOptions.html)

[ICWResults::SetPlotDisplayOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotDisplayOptions.html)

[ICWResults::SetPlotSettings Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotSettings.html)

[ICWResults::AddIsoClippingToPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~AddIsoClippingToPlot.html)

[ICWResults::CreatePlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreatePlot.html)

[ICWResults::SetPlotSettingsOptionForHiddenAndExcludedBody Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotSettingsOptionForHiddenAndExcludedBody.html)

[ICWResults::CreateResultsEquationPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateResultsEquationPlot.html)

[ICWResults::GetPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlot.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0