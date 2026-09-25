<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~RunThickAnalysis2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| RunThickAnalysis2 Method (IThicknessAnalysis) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IThicknessAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis.html) : RunThickAnalysis2 Method (IThicknessAnalysis) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*targetthickness*
:   Target thickness in meters

*thicklimit*
:   Thickness region limit in meters

*treatcornerzero*
:   True to disregard corners sharp corners, false to not

*resolution*
:   Resolution as defined in [gttckResolutionOptions\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gttckResolutionOptions_e.html)

*lResultOptions*
:   Display the results or save results to a report as defined in [gtResultOptions\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtResultOptions_e.html)

*reportname*
:   Path where to save the results report

*vtAddToBinderOption*
:   True to add the results report to the Design Binder, false to not

*vtSaveResultsInEdwg*
:   True to save the results in eDrawings, false to not

*vtOverwrite*
:   True to overwrite an existing results report of the same name, false to not

Runs a thickness analysis, shows the thick regions, and generates a report.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RunThickAnalysis2( _    ByVal targetthickness As System.Double, _    ByVal thicklimit As System.Double, _    ByVal treatcornerzero As System.Boolean, _    ByVal resolution As System.Integer, _    ByVal lResultOptions As System.Integer, _    ByVal reportname As System.String, _    ByVal vtAddToBinderOption As System.Boolean, _    ByVal vtSaveResultsInEdwg As System.Boolean, _    ByVal vtOverwrite As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IThicknessAnalysis Dim targetthickness As System.Double Dim thicklimit As System.Double Dim treatcornerzero As System.Boolean Dim resolution As System.Integer Dim lResultOptions As System.Integer Dim reportname As System.String Dim vtAddToBinderOption As System.Boolean Dim vtSaveResultsInEdwg As System.Boolean Dim vtOverwrite As System.Boolean Dim value As System.Integer   value = instance.RunThickAnalysis2(targetthickness, thicklimit, treatcornerzero, resolution, lResultOptions, reportname, vtAddToBinderOption, vtSaveResultsInEdwg, vtOverwrite) ``` | |

| C# |  |
| --- | --- |
| ``` System.int RunThickAnalysis2(     System.double targetthickness,    System.double thicklimit,    System.bool treatcornerzero,    System.int resolution,    System.int lResultOptions,    System.string reportname,    System.bool vtAddToBinderOption,    System.bool vtSaveResultsInEdwg,    System.bool vtOverwrite ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int RunThickAnalysis2(  &   System.double targetthickness, &   System.double thicklimit, &   System.bool treatcornerzero, &   System.int resolution, &   System.int lResultOptions, &   System.String^ reportname, &   System.bool vtAddToBinderOption, &   System.bool vtSaveResultsInEdwg, &   System.bool vtOverwrite ) ``` | |

#### Parameters

*targetthickness*
:   Target thickness in meters

*thicklimit*
:   Thickness region limit in meters

*treatcornerzero*
:   True to disregard corners sharp corners, false to not

*resolution*
:   Resolution as defined in [gttckResolutionOptions\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gttckResolutionOptions_e.html)

*lResultOptions*
:   Display the results or save results to a report as defined in [gtResultOptions\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtResultOptions_e.html)

*reportname*
:   Path where to save the results report

*vtAddToBinderOption*
:   True to add the results report to the Design Binder, false to not

*vtSaveResultsInEdwg*
:   True to save the results in eDrawings, false to not

*vtOverwrite*
:   True to overwrite an existing results report of the same name, false to not

#### Return Value

Error as defined in [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IThicknessAnalysis::RunThickAnalysis2.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **If there are any...** | **Then the analysis is run on...** |
| Selected faces | Only those faces |
| Selected faces that belong to multiple solid bodies | Only on the selected faces of the body selected by IThicknessAnalysys::SetThicknessAnalysisBody |

# ![](dotnetimages/collapse.gif)See Also

####

[IThicknessAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis.html)

[IThicknessAnalysis Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis_members.html)

[IThickAnalysis::RunThinAnalysis2 Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~RunThinAnalysis2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2007 FCS