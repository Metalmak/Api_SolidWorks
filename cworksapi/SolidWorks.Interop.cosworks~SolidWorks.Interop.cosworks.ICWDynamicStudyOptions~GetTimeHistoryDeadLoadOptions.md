<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetTimeHistoryDeadLoadOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetTimeHistoryDeadLoadOptions Method (ICWDynamicStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html) : GetTimeHistoryDeadLoadOptions Method (ICWDynamicStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BChecked*
:   1 to get dead loads from a static study, 0 to not

*SStudyName*
:   Name of the static study

*DMultiplicationFactor*
:   Multiplication factor

Obsolete. Superseded by [ICWDynamicStudyOptions::GetTimeHistoryDeadLoadOptions2.](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicStudyOptions~GetTimeHistoryDeadLoadOptions2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetTimeHistoryDeadLoadOptions( _    ByRef BChecked As System.Integer, _    ByRef SStudyName As System.String, _    ByRef DMultiplicationFactor As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicStudyOptions Dim BChecked As System.Integer Dim SStudyName As System.String Dim DMultiplicationFactor As System.Double   instance.GetTimeHistoryDeadLoadOptions(BChecked, SStudyName, DMultiplicationFactor) ``` | |

| C# |  |
| --- | --- |
| ``` void GetTimeHistoryDeadLoadOptions(     out System.int BChecked,    out System.string SStudyName,    out System.double DMultiplicationFactor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetTimeHistoryDeadLoadOptions(  &   [Out] System.int BChecked, &   [Out] System.String^ SStudyName, &   [Out] System.double DMultiplicationFactor ) ``` | |

#### Parameters

*BChecked*
:   1 to get dead loads from a static study, 0 to not

*SStudyName*
:   Name of the static study

*DMultiplicationFactor*
:   Multiplication factor

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDynamicStudyOptions::GetTimeHistoryDeadLoadOptions.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html)

[ICWDynamicStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions_members.html)

[ICWDynamicStudyOptions::SetTimeHistoryDeadLoadOptions Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetTimeHistoryDeadLoadOptions.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0