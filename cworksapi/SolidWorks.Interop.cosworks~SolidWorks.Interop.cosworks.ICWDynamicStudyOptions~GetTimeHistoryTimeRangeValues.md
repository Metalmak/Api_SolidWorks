<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetTimeHistoryTimeRangeValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetTimeHistoryTimeRangeValues Method (ICWDynamicStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html) : GetTimeHistoryTimeRangeValues Method (ICWDynamicStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DStartTime*
:   Start time

*DEndTime*
:   End time

*DTimeIncrement*
:   Time increment

Obsolete. Superseded by [ICWDynamicStudyOptions::GetTimeHistoryTimeRangeValues2.](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicStudyOptions~GetTimeHistoryTimeRangeValues2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetTimeHistoryTimeRangeValues( _    ByRef DStartTime As System.Double, _    ByRef DEndTime As System.Double, _    ByRef DTimeIncrement As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicStudyOptions Dim DStartTime As System.Double Dim DEndTime As System.Double Dim DTimeIncrement As System.Double   instance.GetTimeHistoryTimeRangeValues(DStartTime, DEndTime, DTimeIncrement) ``` | |

| C# |  |
| --- | --- |
| ``` void GetTimeHistoryTimeRangeValues(     out System.double DStartTime,    out System.double DEndTime,    out System.double DTimeIncrement ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetTimeHistoryTimeRangeValues(  &   [Out] System.double DStartTime, &   [Out] System.double DEndTime, &   [Out] System.double DTimeIncrement ) ``` | |

#### Parameters

*DStartTime*
:   Start time

*DEndTime*
:   End time

*DTimeIncrement*
:   Time increment

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDynamicStudyOptions::GetTimeHistoryTimeRangeValues.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html)

[ICWDynamicStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions_members.html)

[ICWDynamicStudyOptions::SetTimeHistoryTimeRangeValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetTimeHistoryTimeRangeValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0