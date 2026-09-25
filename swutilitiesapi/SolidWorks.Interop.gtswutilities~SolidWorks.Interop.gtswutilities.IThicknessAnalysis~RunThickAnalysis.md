<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~RunThickAnalysis.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| RunThickAnalysis Method (IThicknessAnalysis) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IThicknessAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis.html) : RunThickAnalysis Method (IThicknessAnalysis) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*targetthickness*

*thicklimit*

*treatcornerzero*

*resolution*

*lResultOptions*

*reportname*

*vtAddToBinderOption*

*vtOverwrite*

Obsolete. Superseded by [IThicknessAnalysis::RunThickAnalysis2](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IThicknessAnalysis~RunThickAnalysis2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RunThickAnalysis( _    ByVal targetthickness As System.Double, _    ByVal thicklimit As System.Double, _    ByVal treatcornerzero As System.Boolean, _    ByVal resolution As System.Integer, _    ByVal lResultOptions As System.Integer, _    ByVal reportname As System.String, _    ByVal vtAddToBinderOption As System.Boolean, _    ByVal vtOverwrite As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IThicknessAnalysis Dim targetthickness As System.Double Dim thicklimit As System.Double Dim treatcornerzero As System.Boolean Dim resolution As System.Integer Dim lResultOptions As System.Integer Dim reportname As System.String Dim vtAddToBinderOption As System.Boolean Dim vtOverwrite As System.Boolean Dim value As System.Integer   value = instance.RunThickAnalysis(targetthickness, thicklimit, treatcornerzero, resolution, lResultOptions, reportname, vtAddToBinderOption, vtOverwrite) ``` | |

| C# |  |
| --- | --- |
| ``` System.int RunThickAnalysis(     System.double targetthickness,    System.double thicklimit,    System.bool treatcornerzero,    System.int resolution,    System.int lResultOptions,    System.string reportname,    System.bool vtAddToBinderOption,    System.bool vtOverwrite ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int RunThickAnalysis(  &   System.double targetthickness, &   System.double thicklimit, &   System.bool treatcornerzero, &   System.int resolution, &   System.int lResultOptions, &   System.String^ reportname, &   System.bool vtAddToBinderOption, &   System.bool vtOverwrite ) ``` | |

#### Parameters

*targetthickness*

*thicklimit*

*treatcornerzero*

*resolution*

*lResultOptions*

*reportname*

*vtAddToBinderOption*

*vtOverwrite*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IThicknessAnalysis::RunThickAnalysis.

# ![](dotnetimages/collapse.gif)See Also

####

[IThicknessAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis.html)

[IThicknessAnalysis Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis_members.html)