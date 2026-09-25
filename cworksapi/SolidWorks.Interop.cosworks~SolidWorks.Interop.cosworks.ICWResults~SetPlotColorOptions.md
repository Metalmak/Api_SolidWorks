<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotColorOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetPlotColorOptions Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : SetPlotColorOptions Method (ICWResults) |

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

*NType*
:   Color map as defined in [swsColorChartOptionLegendTypeValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsColorChartOptionLegendTypeValue_e.html) (see **Remarks**)

*NContour*
:   2 <= Number of gradient colors <= 24

*NBaseColor*
:   Number of base colors for NType; valid only if NType is swsColorChartOptionLegendTypeValue\_e.swsColorChartOptionLegendUserDefined (see **Remarks**)

*BFlip*
:   True to reverse the color mapping, false to not

*BSpecifyColorLimit*
:   True to specify a color for values above the yield limit, false to not; valid only for von Mises stress plots of single body parts where the yield strength is defined

*VarColor*
:   Array of RGB triplets:

    * RGB color for values above the yield limit; valid only if BSpecifyColorLimit is true* One or more RGB triplets of user-defined colors

Sets the color options for the specified plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPlotColorOptions( _    ByVal SPlotName As System.String, _    ByVal NType As System.Integer, _    ByVal NContour As System.Integer, _    ByVal NBaseColor As System.Integer, _    ByVal BFlip As System.Boolean, _    ByVal BSpecifyColorLimit As System.Boolean, _    ByVal VarColor As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim SPlotName As System.String Dim NType As System.Integer Dim NContour As System.Integer Dim NBaseColor As System.Integer Dim BFlip As System.Boolean Dim BSpecifyColorLimit As System.Boolean Dim VarColor As System.Object Dim value As System.Integer   value = instance.SetPlotColorOptions(SPlotName, NType, NContour, NBaseColor, BFlip, BSpecifyColorLimit, VarColor) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetPlotColorOptions(     System.string SPlotName,    System.int NType,    System.int NContour,    System.int NBaseColor,    System.bool BFlip,    System.bool BSpecifyColorLimit,    System.object VarColor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetPlotColorOptions(  &   System.String^ SPlotName, &   System.int NType, &   System.int NContour, &   System.int NBaseColor, &   System.bool BFlip, &   System.bool BSpecifyColorLimit, &   System.Object^ VarColor ) ``` | |

#### Parameters

*SPlotName*
:   Plot name (see **Remarks**)

*NType*
:   Color map as defined in [swsColorChartOptionLegendTypeValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsColorChartOptionLegendTypeValue_e.html) (see **Remarks**)

*NContour*
:   2 <= Number of gradient colors <= 24

*NBaseColor*
:   Number of base colors for NType; valid only if NType is swsColorChartOptionLegendTypeValue\_e.swsColorChartOptionLegendUserDefined (see **Remarks**)

*BFlip*
:   True to reverse the color mapping, false to not

*BSpecifyColorLimit*
:   True to specify a color for values above the yield limit, false to not; valid only for von Mises stress plots of single body parts where the yield strength is defined

*VarColor*
:   Array of RGB triplets:

    * RGB color for values above the yield limit; valid only if BSpecifyColorLimit is true* One or more RGB triplets of user-defined colors

#### Return Value

Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::SetPlotColorOptions.

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWResults::GetPlotNames](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotNames.html) to populate SPlotName.

| If NType is swsColorChartOptionLegendTypeValue\_e... | Then NBaseColor is... |
| --- | --- |
| swsColorChartOptionLegendDefault | 5 |
| swsColorChartOptionLegendRainbow | 7 |
| swsColorChartOptionLegendGrayScale | 2 |
| swsColorChartOptionLegendUserDefined | 2-9 |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetPlotColorOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotColorOptions.html)

[ICWResults::SetPlotDisplayOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotDisplayOptions.html)

[ICWResults::SetPlotPositionFormatOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotPositionFormatOptions.html)

[ICWResults::SetPlotSettings Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotSettings.html)

[ICWResults::AddIsoClippingToPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~AddIsoClippingToPlot.html)

[ICWResults::CreatePlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreatePlot.html)

[ICWResults::SetPlotSettingsOptionForHiddenAndExcludedBody Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotSettingsOptionForHiddenAndExcludedBody.html)

[ICWResults::CreateResultsEquationPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateResultsEquationPlot.html)

[ICWResults::GetPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlot.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0