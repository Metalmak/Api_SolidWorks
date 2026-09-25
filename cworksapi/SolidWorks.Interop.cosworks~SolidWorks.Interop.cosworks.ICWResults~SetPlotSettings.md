<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotSettings.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetPlotSettings Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : SetPlotSettings Method (ICWResults) |

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
:   Array of plot settings (see **Remarks**)

Sets various settings for the specified plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPlotSettings( _    ByVal SPlotName As System.String, _    ByVal ArrayInput As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim SPlotName As System.String Dim ArrayInput As System.Object Dim value As System.Integer   value = instance.SetPlotSettings(SPlotName, ArrayInput) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetPlotSettings(     System.string SPlotName,    System.object ArrayInput ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetPlotSettings(  &   System.String^ SPlotName, &   System.Object^ ArrayInput ) ``` | |

#### Parameters

*SPlotName*
:   Plot name (see **Remarks**)

*ArrayInput*
:   Array of plot settings (see **Remarks**)

#### Return Value

Error code as defined in [swsPlotSettingsErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotSettingsErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::SetPlotSettings.

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWResults::GetPlotNames](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotNames.html) to populate SPlotName.

The 0-based array contains 11 elements:

| Array element... | Contains... |
| --- | --- |
| 0 | Display option for active fringe plot as defined in [swsPlotFringeSettingsOptionValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotFringeSettingsOptionValue_e.html) |
| 1 | Display option for model boundary as defined in [swsPlotBoundarySettingsOptionValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotBoundarySettingsOptionValue_e.html) |
| 2 | R[0-255] value for model/mesh color; valid only if array element 1 is not swsPlotBoundarySettingsOptionValue\_e.swsPlotBoundaryNone |
| 3 | G[0-255] value for model/mesh color; valid only if array element 1 is not swsPlotBoundarySettingsOptionValue\_e.swsPlotBoundaryNone |
| 4 | B[0-255] value for model/mesh color; valid only if array element 1 is not swsPlotBoundarySettingsOptionValue\_e.swsPlotBoundaryNone |
| 5 | Boolean; whether to superimpose the undeformed model on the deformed model |
| 6 | Deformed plot translucent color option as defined in [swsPlotDeformedShapeOptionSuperImposeValue\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotDeformedShapeOptionSuperImposeValue_e.html); valid only if array element 5 is true |
| 7 | R[0-255] value for single translucent color; valid only if array elmeent 5 is true, and array element 6 is swsPlotDeformedShapeOptionSuperImposeValue\_e.swsPlotDeformedShapeSuperImposeModel\_TranslucentSingleColor |
| 8 | G[0-255] value for single translucent color; valid only if array element 5 is true, and array element 6 is swsPlotDeformedShapeOptionSuperImposeValue\_e.swsPlotDeformedShapeSuperImposeModel\_TranslucentSingleColor |
| 9 | B[0-255] value for single translucent color; valid only if array element 5 is true, and array element 6 is swsPlotDeformedShapeOptionSuperImposeValue\_e.swsPlotDeformedShapeSuperImposeModel\_TranslucentSingleColor |
| 10 | 0.0 <= Transparency or intensity of the translucent single color or part colors <= 1.0; valid only if array element 5 is true |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetPlotSettings Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotSettings.html)

[ICWResults::SetPlotColorOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotColorOptions.html)

[ICWResults::SetPlotDisplayOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotDisplayOptions.html)

[ICWResults::SetPlotPositionFormatOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotPositionFormatOptions.html)

[ICWResults::AddIsoClippingToPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~AddIsoClippingToPlot.html)

[ICWResults::CreatePlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreatePlot.html)

[ICWResults::SetPlotSettingsOptionForHiddenAndExcludedBody Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotSettingsOptionForHiddenAndExcludedBody.html)

[ICWResults::CreateResultsEquationPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateResultsEquationPlot.html)

[ICWResults::GetPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlot.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0