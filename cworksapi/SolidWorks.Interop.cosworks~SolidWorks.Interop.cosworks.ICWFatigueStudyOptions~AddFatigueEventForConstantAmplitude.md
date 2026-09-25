<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~AddFatigueEventForConstantAmplitude.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddFatigueEventForConstantAmplitude Method (ICWFatigueStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWFatigueStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions.html) : AddFatigueEventForConstantAmplitude Method (ICWFatigueStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SAssociatedStudyName*
:   Name of the reference study (see **Remarks**)

*DScale*
:   0.0 <= Factor by which to scale the result stresses of SAssociatedStudyName <= 1.0E36

*NStep*
:   Solution step of SAssociatedStudyName; valid only for nonlinear or linear dynamic studies

*ErrorCode*
:   Error code as defined in [swsFatigueEventEndEditError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueEventEndEditError_e.html)

Adds a fatigue event to a linear dynamic constant amplitude study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddFatigueEventForConstantAmplitude( _    ByVal SAssociatedStudyName As System.String, _    ByVal DScale As System.Double, _    ByVal NStep As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As CWFatigueEvent ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWFatigueStudyOptions Dim SAssociatedStudyName As System.String Dim DScale As System.Double Dim NStep As System.Integer Dim ErrorCode As System.Integer Dim value As CWFatigueEvent   value = instance.AddFatigueEventForConstantAmplitude(SAssociatedStudyName, DScale, NStep, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWFatigueEvent AddFatigueEventForConstantAmplitude(     System.string SAssociatedStudyName,    System.double DScale,    System.int NStep,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWFatigueEvent^ AddFatigueEventForConstantAmplitude(  &   System.String^ SAssociatedStudyName, &   System.double DScale, &   System.int NStep, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*SAssociatedStudyName*
:   Name of the reference study (see **Remarks**)

*DScale*
:   0.0 <= Factor by which to scale the result stresses of SAssociatedStudyName <= 1.0E36

*NStep*
:   Solution step of SAssociatedStudyName; valid only for nonlinear or linear dynamic studies

*ErrorCode*
:   Error code as defined in [swsFatigueEventEndEditError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueEventEndEditError_e.html)

#### Return Value

[ICWFatigueEvent](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWFatigueEvent.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWFatigueStudyOptions::AddFatigueEventForConstantAmplitude.

# ![](dotnetimages/collapse.gif)Example

See the [ICWFatigueStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

SAssociatedStudyName must be the name of a study of the following type:

* Static* Nonlinear

 -or -

* Linear dynamic time History

To get or set the interaction option for this event, call [ICWFatigueStudyOptions::ConstantAmplitudeEventInteractionOption](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~ConstantAmplitudeEventInteractionOption.html).

To fully configure the constant amplitude fatigue study for this event, call:

* [ICWFatigueStudyOptions::ComputingAlternatingStressOption](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~ComputingAlternatingStressOption.html)* [ICWFatigueStudyOptions::FatigueStrengthReductionFactor](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~FatigueStrengthReductionFactor.html)* [ICWFatigueStudyOptions::MeanStressCorrectionOption](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~MeanStressCorrectionOption.html)* [ICWFatigueStudyOptions::ResultFolder](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~ResultFolder.html)* [ICWFatigueStudyOptions::ShellFace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~ShellFace.html)* [ICWFatigueStudyOptions::SetInfiniteLifeSettings](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~SetInfiniteLifeSettings.html)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWFatigueStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions.html)

[ICWFatigueStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions_members.html)

[ICWFatigueStudyOptions::AddFatigueEventForHarmonic Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~AddFatigueEventForHarmonic.html)

[ICWFatigueStudyOptions::AddFatigueEventForRandomVibration Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~AddFatigueEventForRandomVibration.html)

[ICWFatigueStudyOptions::AddFatigueEventForVariableAmplitude Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~AddFatigueEventForVariableAmplitude.html)

[ICWFatigueStudyOptions::DeleteFatigueEvent Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~DeleteFatigueEvent.html)

[ICWFatigueStudyOptions::GetFatigueEvent Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~GetFatigueEvent.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0