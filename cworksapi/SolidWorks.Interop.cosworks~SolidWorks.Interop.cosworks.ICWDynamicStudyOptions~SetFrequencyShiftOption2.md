<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetFrequencyShiftOption2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetFrequencyShiftOption2 Method (ICWDynamicStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html) : SetFrequencyShiftOption2 Method (ICWDynamicStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BChecked*
:   True to only calculate resonant frequencies that are closest to DFrequencyValue, false to not

*DFrequencyValue*
:   Frequency in Hz; valid only if BChecked = true (see **Remarks**)

Sets whether to only calculate resonant frequencies that are closest to a specific frequency.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetFrequencyShiftOption2( _    ByVal BChecked As System.Boolean, _    ByVal DFrequencyValue As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicStudyOptions Dim BChecked As System.Boolean Dim DFrequencyValue As System.Double Dim value As System.Integer   value = instance.SetFrequencyShiftOption2(BChecked, DFrequencyValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetFrequencyShiftOption2(     System.bool BChecked,    System.double DFrequencyValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetFrequencyShiftOption2(  &   System.bool BChecked, &   System.double DFrequencyValue ) ``` | |

#### Parameters

*BChecked*
:   True to only calculate resonant frequencies that are closest to DFrequencyValue, false to not

*DFrequencyValue*
:   Frequency in Hz; valid only if BChecked = true (see **Remarks**)

#### Return Value

0 indicates success; a non-0 value indicates failure

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDynamicStudyOptions::SetFrequencyShiftOption2.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if both of the following are true:

* [ICWDynamicStudyOptions::SolverType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicStudyOptions~SolverType.html) = [swsSolverType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSolverType_e.html).swsSolverTypeDirectSparse* [ICWDynamicStudyOptions::GetFrequencyOption2](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicStudyOptions~GetFrequencyOption2.html) = [swsFrequencyStudyOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFrequencyStudyOption_e.html).swsFrequencyStudyOptionNumberFrequencies

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html)

[ICWDynamicStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions_members.html)

[ICWDynamicStudyOptions::GetFrequencyShiftOption2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetFrequencyShiftOption2.html)

[ICWDynamicStudyOptions::SetFrequencyOption2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetFrequencyOption2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0