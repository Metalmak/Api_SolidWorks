<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotColorOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetPlotColorOptions Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetPlotColorOptions Method (ICWResults) |

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

*NBaseColor*
:   Number of base colors in color map specified by NType (see **Remarks**)

*NContour*
:   Number of gradient colors

*BFlip*
:   True to reverse the color mapping, false to not

*BSpecifyColorLimit*
:   True to specify a color for values above the yield limit, false to not; valid only for von Mises stress plots of single body parts where the yield strength is defined

*VarColor*
:   Array of RGB triplets:

    * RGB color for values above the yield limit; valid only if BSpecifyColorLimit is true* One or more RGB triplets of user-defined colors

Gets the color options for the specified plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPlotColorOptions( _    ByVal SPlotName As System.String, _    ByRef NType As System.Integer, _    ByRef NBaseColor As System.Integer, _    ByRef NContour As System.Integer, _    ByRef BFlip As System.Boolean, _    ByRef BSpecifyColorLimit As System.Boolean, _    ByRef VarColor As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim SPlotName As System.String Dim NType As System.Integer Dim NBaseColor As System.Integer Dim NContour As System.Integer Dim BFlip As System.Boolean Dim BSpecifyColorLimit As System.Boolean Dim VarColor As System.Object Dim value As System.Integer   value = instance.GetPlotColorOptions(SPlotName, NType, NBaseColor, NContour, BFlip, BSpecifyColorLimit, VarColor) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetPlotColorOptions(     System.string SPlotName,    out System.int NType,    out System.int NBaseColor,    out System.int NContour,    out System.bool BFlip,    out System.bool BSpecifyColorLimit,    out System.object VarColor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetPlotColorOptions(  &   System.String^ SPlotName, &   [Out] System.int NType, &   [Out] System.int NBaseColor, &   [Out] System.int NContour, &   [Out] System.bool BFlip, &   [Out] System.bool BSpecifyColorLimit, &   [Out] System.Object^ VarColor ) ``` | |

#### Parameters

*SPlotName*
:   Plot name (see **Remarks**)

*NType*
:   Color map as defined in [swsColorChartOptionLegendTypeValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsColorChartOptionLegendTypeValue_e.html) (see **Remarks**)

*NBaseColor*
:   Number of base colors in color map specified by NType (see **Remarks**)

*NContour*
:   Number of gradient colors

*BFlip*
:   True to reverse the color mapping, false to not

*BSpecifyColorLimit*
:   True to specify a color for values above the yield limit, false to not; valid only for von Mises stress plots of single body parts where the yield strength is defined

*VarColor*
:   Array of RGB triplets:

    * RGB color for values above the yield limit; valid only if BSpecifyColorLimit is true* One or more RGB triplets of user-defined colors

#### Return Value

Error as defined in [swsResultsError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetPlotColorOptions.

# ![](dotnetimages/collapse.gif)Example

[Analyze Part (VBA)](Analyze_Part_Example_VB.htm)

[Analyze Part (VB.NET)](Analyze_Part_Example_VBNET.htm)

[Analyze Part (C#)](Analyze_Part_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWResults::GetPlotNames](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotNames.html) to populate SPlotName.

| If NType is swsColorChartOptionLegendTypeValue\_e... | Then NBaseColor is... |
| --- | --- |
| swsColorChartOptionLegendDefault | 5 |
| swsColorChartOptionLegendRainbow | 7 |
| swsColorChartOptionLegendGrayScale | 2 |
| swsColorChartOptionLegendUserDefined | 2 - 9 |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::SetPlotColorOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotColorOptions.html)

[ICWResults::GetPlotCount Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotCount.html)

[ICWResults::GetPlotDisplayOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotDisplayOptions.html)

[ICWResults::GetPlotPositionFormatOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotPositionFormatOptions.html)

[ICWResults::GetPlotSettings Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotSettings.html)

[ICWResults::CreatePlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreatePlot.html)

[ICWResults::GetLegendContourColors Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetLegendContourColors.html)

[ICWResults::GetPlotSettingsOptionForHiddenAndExcludedBody Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotSettingsOptionForHiddenAndExcludedBody.html)

[ICWResults::CreateResultsEquationPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateResultsEquationPlot.html)

[ICWResults::GetPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlot.html)

[ICWResults::GetPlotDefinition Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotDefinition.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0