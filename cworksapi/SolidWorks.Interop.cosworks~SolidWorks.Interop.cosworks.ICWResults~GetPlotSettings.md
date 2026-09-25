<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotSettings.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetPlotSettings Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetPlotSettings Method (ICWResults) |

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

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Gets the settings for the specified plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPlotSettings( _    ByVal SPlotName As System.String, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim SPlotName As System.String Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetPlotSettings(SPlotName, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetPlotSettings(     System.string SPlotName,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetPlotSettings(  &   System.String^ SPlotName, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*SPlotName*
:   Plot name (see **Remarks**)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

#### Return Value

Array of plot settings (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetPlotSettings.

# ![](dotnetimages/collapse.gif)Example

[Analyze Part (VBA)](Analyze_Part_Example_VB.htm)

[Analyze Part (VB.NET)](Analyze_Part_Example_VBNET.htm)

[Analyze Part (C#)](Analyze_Part_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWResults::GetPlotNames](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotNames.html) to populate SPlotName.

The 0-based array contains 11 elements:

| Array element... | Contains... |
| --- | --- |
| 0 | Display option for active fringe plot as defined in [swsPlotFringeSettingsOptionValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotFringeSettingsOptionValue_e.html) |
| 1 | Display option for model boundary as defined in [swsPlotBoundarySettingsOptionValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotBoundarySettingsOptionValue_e.html) |
| 2 | R[0-255] value for model/mesh color; valid only if array element 1 is not swsPlotBoundarySettingsOptionValue\_e.swsPlotBoundaryNone |
| 3 | G[0-255] value for model/mesh color; valid only if array element 1 is not swsPlotBoundarySettingsOptionValue\_e.swsPlotBoundaryNone |
| 4 | B[0-255] value for model/mesh color; valid only if array element 1 is not swsPlotBoundarySettingsOptionValue\_e.swsPlotBoundaryNone |
| 5 | Boolean; whether to superimpose the undeformed model on the deformed model |
| 6 | Deformed plot translucent color option as defined in [swsPlotDeformedShapeOptionSuperImposeValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotDeformedShapeOptionSuperImposeValue_e.html); valid only if array element 5 is true |
| 7 | R[0-255] value for single translucent color; valid only if array element 5 is true, and array element 6 is swsPlotDeformedShapeOptionSuperImposeValue\_e.swsPlotDeformedShapeSuperImposeModel\_TranslucentSingleColor |
| 8 | G[0-255] value for single translucent color; valid only if array element 5 is true, and array element 6 is swsPlotDeformedShapeOptionSuperImposeValue\_e.swsPlotDeformedShapeSuperImposeModel\_TranslucentSingleColor |
| 9 | B[0-255] value for single translucent color; valid only if array element 5 is true, and array element 6is swsPlotDeformedShapeOptionSuperImposeValue\_e.swsPlotDeformedShapeSuperImposeModel\_TranslucentSingleColor |
| 10 | 0.0 <= Transparency or intensity of the translucent single color or part colors <= 1.0; valid only if array element 5 is true |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::SetPlotSettings Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotSettings.html)

[ICWResults::GetPlotColorOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotColorOptions.html)

[ICWResults::GetPlotCount Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotCount.html)

[ICWResults::GetPlotDisplayOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotDisplayOptions.html)

[ICWResults::GetPlotPositionFormatOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotPositionFormatOptions.html)

[ICWResults::CreatePlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreatePlot.html)

[ICWResults::GetPlotSettingsOptionForHiddenAndExcludedBody Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotSettingsOptionForHiddenAndExcludedBody.html)

[ICWResults::GetLegendContourColors Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetLegendContourColors.html)

[ICWResults::CreateResultsEquationPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateResultsEquationPlot.html)

[ICWResults::GetPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlot.html)

[ICWResults::GetPlotDefinition Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotDefinition.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0