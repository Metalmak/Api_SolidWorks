<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SetSolutionStepsSetInformation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetSolutionStepsSetInformation Method (ICWStudyResultOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html) : SetSolutionStepsSetInformation Method (ICWStudyResultOptions) |

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

Sets solution steps set information.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSolutionStepsSetInformation( _    ByVal NSetNumber As System.Integer, _    ByVal NStartStep As System.Integer, _    ByVal NEndStep As System.Integer, _    ByVal NStepIncrement As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyResultOptions Dim NSetNumber As System.Integer Dim NStartStep As System.Integer Dim NEndStep As System.Integer Dim NStepIncrement As System.Integer Dim value As System.Integer   value = instance.SetSolutionStepsSetInformation(NSetNumber, NStartStep, NEndStep, NStepIncrement) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetSolutionStepsSetInformation(     System.int NSetNumber,    System.int NStartStep,    System.int NEndStep,    System.int NStepIncrement ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetSolutionStepsSetInformation(  &   System.int NSetNumber, &   System.int NStartStep, &   System.int NEndStep, &   System.int NStepIncrement ) ``` | |

#### Parameters

*NSetNumber*
:   Solution steps set number (1-5)

*NStartStep*
:   1 <= Starting step <= 10000

*NEndStep*
:   1 <= Ending step <= 10000

*NStepIncrement*
:   1 <= Step increment <= 10000

#### Return Value

Status code as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyResultOptions::SetSolutionStepsSetInformation.

# ![](dotnetimages/collapse.gif)Example

See the [ICWStudyResultOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWStudyResultOptions::SaveResultsForSolutionStepsOption](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWStudyResultOptions~SaveResultsForSolutionStepsOption.html) = [swsSaveResultsOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSaveResultsOption_e.html).swsSaveResultsOption\_ForSpecifiedSolutionSteps.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html)

[ICWStudyResultOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions_members.html)

[ICWStudyResultOptions::GetSolutionStepsSetInformation Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~GetSolutionStepsSetInformation.html)

[ICWStudyResultOptions::SaveResultsForSolutionStepsOption Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SaveResultsForSolutionStepsOption.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0