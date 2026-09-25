<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~TimeHistoryWilsonTheta.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| TimeHistoryWilsonTheta Property (ICWDynamicStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html) : TimeHistoryWilsonTheta Property (ICWDynamicStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [ICWDynamicStudyOptions::GetTimeHistoryWilsonTheta2](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicStudyOptions~GetTimeHistoryWilsonTheta2.html) and [ICWDynamicStudyOptions::SetTimeHistoryWilsonTheta2.](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicStudyOptions~SetTimeHistoryWilsonTheta2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property TimeHistoryWilsonTheta As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicStudyOptions Dim value As System.Double   instance.TimeHistoryWilsonTheta = value   value = instance.TimeHistoryWilsonTheta ``` | |

| C# |  |
| --- | --- |
| ``` System.double TimeHistoryWilsonTheta {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double TimeHistoryWilsonTheta {    System.double get();    void set ( &   System.double value); } ``` | |

#### Property Value

Theta value (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDynamicStudyOptions::TimeHistoryWilsonTheta.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [ICWDynamicStudyOptions::TimeHistoryIntegrationMethod](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicStudyOptions~TimeHistoryIntegrationMethod.html) = 1 (Wilson Theta).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html)

[ICWDynamicStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions_members.html)

[ICWDynamicStudyOptions::TimeHistoryFirstIntegrationParameter Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~TimeHistoryFirstIntegrationParameter.html)

[ICWDynamicStudyOptions::TimeHistorySecondIntegrationParameter Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~TimeHistorySecondIntegrationParameter.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0