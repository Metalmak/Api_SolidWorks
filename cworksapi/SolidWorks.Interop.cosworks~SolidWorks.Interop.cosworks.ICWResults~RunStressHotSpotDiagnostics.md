<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~RunStressHotSpotDiagnostics.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| RunStressHotSpotDiagnostics Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : RunStressHotSpotDiagnostics Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NSensitivityFactor*
:   5 <= Highest equivalent strain percent <= 100

*BRunForNodes*
:   True to run for nodes, false to not (see **Remarks**)

*BFoundHotSpots*
:   True if stress hot spots are found, false if not (see **Remarks**)

Obsolete. Superseded by [ICWResults::RunStressHotSpotDiagnosticsAndDetectSingularities](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~RunStressHotSpotDiagnosticsAndDetectSingularities.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RunStressHotSpotDiagnostics( _    ByVal NSensitivityFactor As System.Integer, _    ByVal BRunForNodes As System.Boolean, _    ByRef BFoundHotSpots As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim NSensitivityFactor As System.Integer Dim BRunForNodes As System.Boolean Dim BFoundHotSpots As System.Boolean Dim value As System.Integer   value = instance.RunStressHotSpotDiagnostics(NSensitivityFactor, BRunForNodes, BFoundHotSpots) ``` | |

| C# |  |
| --- | --- |
| ``` System.int RunStressHotSpotDiagnostics(     System.int NSensitivityFactor,    System.bool BRunForNodes,    out System.bool BFoundHotSpots ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int RunStressHotSpotDiagnostics(  &   System.int NSensitivityFactor, &   System.bool BRunForNodes, &   [Out] System.bool BFoundHotSpots ) ``` | |

#### Parameters

*NSensitivityFactor*
:   5 <= Highest equivalent strain percent <= 100

*BRunForNodes*
:   True to run for nodes, false to not (see **Remarks**)

*BFoundHotSpots*
:   True if stress hot spots are found, false if not (see **Remarks**)

#### Return Value

Error code as defined in [swsRunStressHotSpotDiagnosticsError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRunStressHotSpotDiagnosticsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::RunStressHotSpotDiagnostics.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, you can call:

* [ICWResults::CreateStressHotSpotPlot](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateStressHotSpotPlot.html) and [ICWResults::GetDetectedHotSpotElements](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetDetectedHotSpotElements.html) if BRunForNodes is false.* [ICWResults::GetDetectedHotSpotNodes](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetDetectedHotSpotNodes.html) if BRunForNodes is true.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0