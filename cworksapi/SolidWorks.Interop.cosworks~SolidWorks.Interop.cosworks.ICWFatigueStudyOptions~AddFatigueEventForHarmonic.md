<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~AddFatigueEventForHarmonic.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddFatigueEventForHarmonic Method (ICWFatigueStudyOptions) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWFatigueStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions.html) : AddFatigueEventForHarmonic Method (ICWFatigueStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SAssociatedStudyName*
:   Name of the reference linear dynamic harmonic study (see **Remarks**)

*DFrequency*
:   Frequency of SAssociatedStudyName; valid only if NPlotStep is 0

*NPlotStep*
:   Solution step number of SAssociatedStudyName; valid only if DFrequency is 0

*DCycles*
:   1.0 < Number of cycles associated with this event < 1.0E36

*DScale*
:   0.0 <= Factor by which to scale the result stresses of SAssociatedStudyName to produce fatigue <= 1.0E36

*ErrorCode*
:   Error code as defined in [swsFatigueEventEndEditError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueEventEndEditError_e.html)

Adds a fatigue event to a linear dynamic harmonic study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddFatigueEventForHarmonic( _    ByVal SAssociatedStudyName As System.String, _    ByVal DFrequency As System.Double, _    ByVal NPlotStep As System.Integer, _    ByVal DCycles As System.Double, _    ByVal DScale As System.Double, _    ByRef ErrorCode As System.Integer _ ) As CWFatigueEvent ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWFatigueStudyOptions Dim SAssociatedStudyName As System.String Dim DFrequency As System.Double Dim NPlotStep As System.Integer Dim DCycles As System.Double Dim DScale As System.Double Dim ErrorCode As System.Integer Dim value As CWFatigueEvent   value = instance.AddFatigueEventForHarmonic(SAssociatedStudyName, DFrequency, NPlotStep, DCycles, DScale, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWFatigueEvent AddFatigueEventForHarmonic(     System.string SAssociatedStudyName,    System.double DFrequency,    System.int NPlotStep,    System.double DCycles,    System.double DScale,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWFatigueEvent^ AddFatigueEventForHarmonic(  &   System.String^ SAssociatedStudyName, &   System.double DFrequency, &   System.int NPlotStep, &   System.double DCycles, &   System.double DScale, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*SAssociatedStudyName*
:   Name of the reference linear dynamic harmonic study (see **Remarks**)

*DFrequency*
:   Frequency of SAssociatedStudyName; valid only if NPlotStep is 0

*NPlotStep*
:   Solution step number of SAssociatedStudyName; valid only if DFrequency is 0

*DCycles*
:   1.0 < Number of cycles associated with this event < 1.0E36

*DScale*
:   0.0 <= Factor by which to scale the result stresses of SAssociatedStudyName to produce fatigue <= 1.0E36

*ErrorCode*
:   Error code as defined in [swsFatigueEventEndEditError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueEventEndEditError_e.html)

#### Return Value

[ICWFatigueEvent](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWFatigueEvent.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWFatigueStudyOptions::AddFatigueEventForHarmonic.

# ![](dotnetimages/collapse.gif)Example

[Create Fatigue Study for Dynamic Harmonic Study (VBA)](Create_Fatigue_Study_for_Dynamic_Harmonic_Study_Example_VB.htm)

[Create Fatigue Study for Dynamic Harmonic Study (VB.NET)](Create_Fatigue_Study_for_Dynamic_Harmonic_Study_Example_VBNET.htm)

[Create Fatigue Study for Dynamic Harmonic Study (C#)](Create_Fatigue_Study_for_Dynamic_Harmonic_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method works only in SOLIDWORKS Simulation Premium.

Before running a fatigue harmonic study, apply material with defined fatigue S-N curves to the model parts of SAssociatedStudyName.

To fully configure the harmonic fatigue study for this event, call:

* [ICWFatigueStudyOptions::FatigueStrengthReductionFactor](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~FatigueStrengthReductionFactor.html)* [ICWFatigueStudyOptions::ResultFolder](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~ResultFolder.html)* [ICWFatigueStudyOptions::ShellFace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~ShellFace.html)* [ICWFatigueStudyOptions::SetInfiniteLifeSettings](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~SetInfiniteLifeSettings.html)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWFatigueStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions.html)

[ICWFatigueStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions_members.html)

[ICWFatigueStudyOptions::AddFatigueEventForConstantAmplitude Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~AddFatigueEventForConstantAmplitude.html)

[ICWFatigueStudyOptions::AddFatigueEventForRandomVibration Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~AddFatigueEventForRandomVibration.html)

[ICWFatigueStudyOptions::AddFatigueEventForVariableAmplitude Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~AddFatigueEventForVariableAmplitude.html)

[ICWFatigueStudyOptions::DeleteFatigueEvent Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~DeleteFatigueEvent.html)

[ICWFatigueStudyOptions::GetFatigueEvent Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~GetFatigueEvent.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP3