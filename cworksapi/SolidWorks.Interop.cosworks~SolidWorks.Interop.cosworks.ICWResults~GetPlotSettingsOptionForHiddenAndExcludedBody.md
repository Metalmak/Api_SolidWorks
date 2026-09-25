<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotSettingsOptionForHiddenAndExcludedBody.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetPlotSettingsOptionForHiddenAndExcludedBody Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetPlotSettingsOptionForHiddenAndExcludedBody Method (ICWResults) |

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
:   Error code as defined in [swsPlotSettingsErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotSettingsErrorCode_e.html)

Gets hidden and excluded body options for the specified plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPlotSettingsOptionForHiddenAndExcludedBody( _    ByVal SPlotName As System.String, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim SPlotName As System.String Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetPlotSettingsOptionForHiddenAndExcludedBody(SPlotName, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetPlotSettingsOptionForHiddenAndExcludedBody(     System.string SPlotName,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetPlotSettingsOptionForHiddenAndExcludedBody(  &   System.String^ SPlotName, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*SPlotName*
:   Plot name (see **Remarks**)

*ErrorCode*
:   Error code as defined in [swsPlotSettingsErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotSettingsErrorCode_e.html)

#### Return Value

Array of hidden and excluded body options (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetPlotSettingsOptionForHiddenAndExcludedBody.

# ![](dotnetimages/collapse.gif)Example

[Analyze Part (VBA)](Analyze_Part_Example_VB.htm)

[Analyze Part (VB.NET)](Analyze_Part_Example_VBNET.htm)

[Analyze Part (C#)](Analyze_Part_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWResults::GetPlotNames](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotNames.html) to populate SPlotName.

The 0-based array contains 12 elements:

| Array element... | Contains... |
| --- | --- |
| 0 | Boolean; whether to show hidden bodies |
| 1 | Hidden body translucent color option as defined in [swsPlotShowHiddenBodiesOptionValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotShowHiddenBodiesOptionValue_e.html); valid only if array element 0 is true |
| 2 | R[0-255] value for single translucent color; valid only if array element 0 is true, and array element 1 is swsPlotShowHiddenBodiesOptionValue\_e.swsPlotHiddenBodyTranslucentSingleColor |
| 3 | G[0-255] value for single translucent color; valid only if array element 0 is true, and array element 1 is swsPlotShowHiddenBodiesOptionValue\_e.swsPlotHiddenBodyTranslucentSingleColor |
| 4 | B[0-255] value for single translucent color; valid only if array element 0 is true, and array element 1 is swsPlotShowHiddenBodiesOptionValue\_e.swsPlotHiddenBodyTranslucentSingleColor |
| 5 | 0.0 <= transparency or intensity of the translucent single color or part colors <= 1.0; valid only if array element 0 is true |
| 6 | Boolean; whether to show excluded bodies |
| 7 | Excluded body translucent color option as defined in [swsPlotShowExcludedBodiesOptionValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotShowExcludedBodiesOptionValue_e.html); valid only if array element 6 is true |
| 8 | R[0-255] value for single translucent color; valid only if array element 6 is true, and array element 7 is swsPlotShowExcludedBodiesOptionValue\_e.swsPlotExcludedBodyTranslucentSingleColor |
| 9 | G[0-255] value for single translucent color; valid only if array element 6 is true, and array element 7 is swsPlotShowExcludedBodiesOptionValue\_e.swsPlotExcludedBodyTranslucentSingleColor |
| 10 | B[0-255] value for single translucent color; valid only if array element 6 is true, and array element 7 is swsPlotShowExcludedBodiesOptionValue\_e.swsPlotExcludedBodyTranslucentSingleColor |
| 11 | 0.0 <= transparency or intensity of the translucent single color or part colors <= 1.0; valid only if array element 6 is true |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetPlotSettings Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotSettings.html)

[ICWResults::SetPlotSettingsOptionForHiddenAndExcludedBody Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotSettingsOptionForHiddenAndExcludedBody.html)

[ICWResults::GetPlotColorOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotColorOptions.html)

[ICWResults::GetPlotCount Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotCount.html)

[ICWResults::GetPlotDisplayOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotDisplayOptions.html)

[ICWResults::GetPlotPositionFormatOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotPositionFormatOptions.html)

[ICWResults::CreatePlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreatePlot.html)

[ICWResults::CreateResultsEquationPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateResultsEquationPlot.html)

[ICWResults::GetPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlot.html)

[ICWResults::GetPlotDefinition Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotDefinition.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0