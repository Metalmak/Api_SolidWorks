<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetRandomVibrationPartialCorrelationDetails2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetRandomVibrationPartialCorrelationDetails2 Method (ICWDynamicStudyOptions) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html) : GetRandomVibrationPartialCorrelationDetails2 Method (ICWDynamicStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NUnits*
:   Units as defined [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*DInRadius*
:   Inside radius

*DOutRadius*
:   Outside radius

Gets the partially correlated units, inside radius, and outside radius for the random vibration dynamic study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetRandomVibrationPartialCorrelationDetails2( _    ByRef NUnits As System.Integer, _    ByRef DInRadius As System.Double, _    ByRef DOutRadius As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicStudyOptions Dim NUnits As System.Integer Dim DInRadius As System.Double Dim DOutRadius As System.Double Dim value As System.Integer   value = instance.GetRandomVibrationPartialCorrelationDetails2(NUnits, DInRadius, DOutRadius) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetRandomVibrationPartialCorrelationDetails2(     out System.int NUnits,    out System.double DInRadius,    out System.double DOutRadius ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetRandomVibrationPartialCorrelationDetails2(  &   [Out] System.int NUnits, &   [Out] System.double DInRadius, &   [Out] System.double DOutRadius ) ``` | |

#### Parameters

*NUnits*
:   Units as defined [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*DInRadius*
:   Inside radius

*DOutRadius*
:   Outside radius

#### Return Value

0 indicates success; a non-0 value indicates failure

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDynamicStudyOptions::GetRandomVibrationPartialCorrelationDetails2.

# ![](dotnetimages/collapse.gif)Example

[Create Linear Dynamic Random Vibration Study (VBA)](Create_Dynamic_Random_Vibration_Study_Example_VB.htm)

[Create Linear Dynamic Random Vibration Study (VB.NET)](Create_Dynamic_Random_Vibration_Study_Example_VBNET.htm)

[Create Linear Dynamic Random Vibration Study (C#)](Create_Dynamic_Random_Vibration_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html)

[ICWDynamicStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions_members.html)

[ICWDynamicStudyOptions::SetRandomVibrationPartialCorrelationDetails2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetRandomVibrationPartialCorrelationDetails2.html)

[ICWDynamicStudyOptions::GetRandomVibrationAnalysisMethod2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetRandomVibrationAnalysisMethod2.html)

[ICWDynamicStudyOptions::GetRandomVibrationBiasingParameter2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetRandomVibrationBiasingParameter2.html)

[ICWDynamicStudyOptions::GetRandomVibrationCorrelationOption2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetRandomVibrationCorrelationOption2.html)

[ICWDynamicStudyOptions::GetRandomVibrationCrossModeCutOffRatio2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetRandomVibrationCrossModeCutOffRatio2.html)

[ICWDynamicStudyOptions::GetRandomVibrationFrequencyLowerLimit2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetRandomVibrationFrequencyLowerLimit2.html)

[ICWDynamicStudyOptions::GetRandomVibrationFrequencyUnits2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetRandomVibrationFrequencyUnits2.html)

[ICWDynamicStudyOptions::GetRandomVibrationFrequencyUpperLimit2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetRandomVibrationFrequencyUpperLimit2.html)

[ICWDynamicStudyOptions::GetRandomVibrationGaussIntegrationOrder2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetRandomVibrationGaussIntegrationOrder2.html)

[ICWDynamicStudyOptions::GetRandomVibrationNoOfFrequencyPoints2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetRandomVibrationNoOfFrequencyPoints2.html)

[ICWDynamicStudyOptions::SetRandomVibrationAnalysisMethod2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetRandomVibrationAnalysisMethod2.html)

[ICWDynamicStudyOptions::SetRandomVibrationBiasingParameter2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetRandomVibrationBiasingParameter2.html)

[ICWDynamicStudyOptions::SetRandomVibrationCorrelationOption2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetRandomVibrationCorrelationOption2.html)

[ICWDynamicStudyOptions::SetRandomVibrationCrossModeCutOffRatio2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetRandomVibrationCrossModeCutOffRatio2.html)

[ICWDynamicStudyOptions::SetRandomVibrationFrequencyLowerLimit2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetRandomVibrationFrequencyLowerLimit2.html)

[ICWDynamicStudyOptions::SetRandomVibrationFrequencyUnits2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetRandomVibrationFrequencyUnits2.html)

[ICWDynamicStudyOptions::SetRandomVibrationFrequencyUpperLimit2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetRandomVibrationFrequencyUpperLimit2.html)

[ICWDynamicStudyOptions::SetRandomVibrationGaussIntegrationOrder2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetRandomVibrationGaussIntegrationOrder2.html)

[ICWDynamicStudyOptions::SetRandomVibrationNoOfFrequencyPoints2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetRandomVibrationNoOfFrequencyPoints2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0