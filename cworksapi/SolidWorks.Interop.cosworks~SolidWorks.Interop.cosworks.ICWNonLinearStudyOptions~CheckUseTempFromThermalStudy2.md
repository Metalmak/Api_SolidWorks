<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~CheckUseTempFromThermalStudy2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CheckUseTempFromThermalStudy2 Property (ICWNonLinearStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) : CheckUseTempFromThermalStudy2 Property (ICWNonLinearStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to use the temperature from the corresponding time of a transient thermal analysis at each nonlinear time step.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property CheckUseTempFromThermalStudy2 As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWNonLinearStudyOptions Dim value As System.Boolean   instance.CheckUseTempFromThermalStudy2 = value   value = instance.CheckUseTempFromThermalStudy2 ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CheckUseTempFromThermalStudy2 {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool CheckUseTempFromThermalStudy2 {    System.bool get();    void set ( &   System.bool value); } ``` | |

#### Property Value

-1 or true to use the temperature from the corresponding time of a transient thermal analysis at each nonlinear time step, 0 or false to not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWNonLinearStudyOptions::CheckUseTempFromThermalStudy2.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if:

* [ICWNonLinearStudyOptions::ThermalResults](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~ThermalResults.html) is set to [swsThermalOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsThermalOption_e.html).swsThermalOption\_TemperatureFromThermalStudy.* [ICWNonLinearStudyOptions::ThermalStudyName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~ThermalStudyName.html) is specified and is a transient thermal study.

This property returns a boolean value which can be cast to an integer. To set this property, you can specify either the boolean or the integer.

If this property is set to false or 0, use [ICWNonLinearStudyOptions::TimeStep](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~TimeStep.html) to specify the time step at which to import a single temperature from a transient thermal study.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html)

[ICWNonLinearStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2021 SP04