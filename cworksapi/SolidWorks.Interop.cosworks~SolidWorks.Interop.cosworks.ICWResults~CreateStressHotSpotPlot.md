<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateStressHotSpotPlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CreateStressHotSpotPlot Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : CreateStressHotSpotPlot Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BIsolateHotSpots*
:   True to isolate stress hot spots, false to not

*BValueByNodes*
:   True to plot node values, false to plot element values

*ErrorCode*
:   Error code as defined in [swsStressHotSpotPlotError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStressHotSpotPlotError_e.html)

Creates a stress hot spot plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateStressHotSpotPlot( _    ByVal BIsolateHotSpots As System.Boolean, _    ByVal BValueByNodes As System.Boolean, _    ByRef ErrorCode As System.Integer _ ) As CWPlot ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim BIsolateHotSpots As System.Boolean Dim BValueByNodes As System.Boolean Dim ErrorCode As System.Integer Dim value As CWPlot   value = instance.CreateStressHotSpotPlot(BIsolateHotSpots, BValueByNodes, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWPlot CreateStressHotSpotPlot(     System.bool BIsolateHotSpots,    System.bool BValueByNodes,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWPlot^ CreateStressHotSpotPlot(  &   System.bool BIsolateHotSpots, &   System.bool BValueByNodes, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*BIsolateHotSpots*
:   True to isolate stress hot spots, false to not

*BValueByNodes*
:   True to plot node values, false to plot element values

*ErrorCode*
:   Error code as defined in [swsStressHotSpotPlotError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStressHotSpotPlotError_e.html)

#### Return Value

[ICWPlot](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::CreateStressHotSpotPlot.

# ![](dotnetimages/collapse.gif)Example

See the [ICWStaticStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must call [ICWResults::RunStressHotSpotDiagnostics](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~RunStressHotSpotDiagnostics.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetDetectedHotSpotElements Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetDetectedHotSpotElements.html)

[ICWResults::GetDetectedHotSpotNodes Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetDetectedHotSpotNodes.html)

[ICWResults::CreatePlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreatePlot.html)

[ICWResults::CreateResultsEquationPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateResultsEquationPlot.html)

[ICWResults::ActivatePlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~ActivatePlot.html)

[ICWResults::GetPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlot.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0