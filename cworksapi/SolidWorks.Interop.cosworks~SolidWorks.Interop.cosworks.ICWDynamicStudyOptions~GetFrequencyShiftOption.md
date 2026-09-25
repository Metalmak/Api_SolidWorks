<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetFrequencyShiftOption.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetFrequencyShiftOption Method (ICWDynamicStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html) : GetFrequencyShiftOption Method (ICWDynamicStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BChecked*
:   True to calculate only resonant frequencies that are closest to DFrequencyValue, false to not

*DFrequencyValue*
:   Frequency in Hz; valid only if BChecked = true (see **Remarks**)

Obsolete. Superseded by [ICWDynamicStudyOptions::GetFrequencyShiftOption2.](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicStudyOptions~GetFrequencyShiftOption2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetFrequencyShiftOption( _    ByRef BChecked As System.Boolean, _    ByRef DFrequencyValue As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicStudyOptions Dim BChecked As System.Boolean Dim DFrequencyValue As System.Double   instance.GetFrequencyShiftOption(BChecked, DFrequencyValue) ``` | |

| C# |  |
| --- | --- |
| ``` void GetFrequencyShiftOption(     out System.bool BChecked,    out System.double DFrequencyValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetFrequencyShiftOption(  &   [Out] System.bool BChecked, &   [Out] System.double DFrequencyValue ) ``` | |

#### Parameters

*BChecked*
:   True to calculate only resonant frequencies that are closest to DFrequencyValue, false to not

*DFrequencyValue*
:   Frequency in Hz; valid only if BChecked = true (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDynamicStudyOptions::GetFrequencyShiftOption.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if both of the following are true:

* [ICWDynamicStudyOptions::SolverType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicStudyOptions~SolverType.html) = swsSolverType\_e.swsSolverTypeDirectSparse* [ICWDynamicStudyOptions::GetFrequencyOption](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicStudyOptions~GetFrequencyOption.html) = swsFrequencyStudyOption\_e.swsFrequencyStudyOptionNumberFrequencies

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html)

[ICWDynamicStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions_members.html)

[ICWDynamicStudyOptions::SetFrequencyShiftOption Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetFrequencyShiftOption.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0