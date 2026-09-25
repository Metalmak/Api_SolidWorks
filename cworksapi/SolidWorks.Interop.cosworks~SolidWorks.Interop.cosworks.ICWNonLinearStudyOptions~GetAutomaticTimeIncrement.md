<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~GetAutomaticTimeIncrement.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetAutomaticTimeIncrement Method (ICWNonLinearStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) : GetAutomaticTimeIncrement Method (ICWNonLinearStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DInitialTimeIncrement*
:   Initial time increment

*DMiNVal*
:   Minimum value

*DMaxVal*
:   Maximum value

*NNoOfAdjustments*
:   Maximum allowed number of adjustments

Gets the parameters for automatic stepping.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetAutomaticTimeIncrement( _    ByRef DInitialTimeIncrement As System.Double, _    ByRef DMiNVal As System.Double, _    ByRef DMaxVal As System.Double, _    ByRef NNoOfAdjustments As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWNonLinearStudyOptions Dim DInitialTimeIncrement As System.Double Dim DMiNVal As System.Double Dim DMaxVal As System.Double Dim NNoOfAdjustments As System.Integer   instance.GetAutomaticTimeIncrement(DInitialTimeIncrement, DMiNVal, DMaxVal, NNoOfAdjustments) ``` | |

| C# |  |
| --- | --- |
| ``` void GetAutomaticTimeIncrement(     out System.double DInitialTimeIncrement,    out System.double DMiNVal,    out System.double DMaxVal,    out System.int NNoOfAdjustments ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetAutomaticTimeIncrement(  &   [Out] System.double DInitialTimeIncrement, &   [Out] System.double DMiNVal, &   [Out] System.double DMaxVal, &   [Out] System.int NNoOfAdjustments ) ``` | |

#### Parameters

*DInitialTimeIncrement*
:   Initial time increment

*DMiNVal*
:   Minimum value

*DMaxVal*
:   Maximum value

*NNoOfAdjustments*
:   Maximum allowed number of adjustments

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWNonLinearStudyOptions::GetAutomaticTimeIncrement.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html)

[ICWNonLinearStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions_members.html)

[ICWNonLinearStudyOptions::SetAutomaticTimeIncrement Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~SetAutomaticTimeIncrement.html)

[ICWNonLinearStudyOptions::EndTime Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~EndTime.html)

[ICWNonLinearStudyOptions::FixedTimeIncrement Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~FixedTimeIncrement.html)

[ICWNonLinearStudyOptions::StartTime Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~StartTime.html)

[ICWNonLinearStudyOptions::TimeIncrement Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~TimeIncrement.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0