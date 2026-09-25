<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~GetSolutionStepsSetInformation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetSolutionStepsSetInformation Method (ICWStudyResultOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html) : GetSolutionStepsSetInformation Method (ICWStudyResultOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NSetNumber*
:   Solution steps set number (1-5)

*NStartStep*
:   1 <= Starting step <= 10000

*NEndStep*
:   1 <= Ending step <= 10000

*NStepIncrement*
:   1 <= Step increment <= 10000

Gets solution steps information for the specified set.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetSolutionStepsSetInformation( _    ByVal NSetNumber As System.Integer, _    ByRef NStartStep As System.Integer, _    ByRef NEndStep As System.Integer, _    ByRef NStepIncrement As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyResultOptions Dim NSetNumber As System.Integer Dim NStartStep As System.Integer Dim NEndStep As System.Integer Dim NStepIncrement As System.Integer   instance.GetSolutionStepsSetInformation(NSetNumber, NStartStep, NEndStep, NStepIncrement) ``` | |

| C# |  |
| --- | --- |
| ``` void GetSolutionStepsSetInformation(     System.int NSetNumber,    out System.int NStartStep,    out System.int NEndStep,    out System.int NStepIncrement ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetSolutionStepsSetInformation(  &   System.int NSetNumber, &   [Out] System.int NStartStep, &   [Out] System.int NEndStep, &   [Out] System.int NStepIncrement ) ``` | |

#### Parameters

*NSetNumber*
:   Solution steps set number (1-5)

*NStartStep*
:   1 <= Starting step <= 10000

*NEndStep*
:   1 <= Ending step <= 10000

*NStepIncrement*
:   1 <= Step increment <= 10000

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyResultOptions::GetSolutionStepsSetInformation.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWStudyResultOptions::SaveResultsForSolutionStepsOption](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWStudyResultOptions~SaveResultsForSolutionStepsOption.html) = swsSaveResultsOption\_e.swsSaveResultsOption\_ForSpecifiedSolutionSteps.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html)

[ICWStudyResultOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions_members.html)

[ICWStudyResultOptions::SetSolutionStepsSetInformation Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SetSolutionStepsSetInformation.html)

[ICWStudyResultOptions::SaveResultsForSolutionStepsOption Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SaveResultsForSolutionStepsOption.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0