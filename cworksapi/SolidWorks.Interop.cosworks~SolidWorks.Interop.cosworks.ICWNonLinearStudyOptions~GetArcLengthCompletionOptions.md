<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~GetArcLengthCompletionOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetArcLengthCompletionOptions Method (ICWNonLinearStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) : GetArcLengthCompletionOptions Method (ICWNonLinearStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DMaxLoad*
:   Maximum load-pattern multiplier

*DMaxDisplacement*
:   Maximum displacement (for translational DOF)

*NUnit*
:   Units as defined in [swsLinearUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinearUnit_e.html)

*NMaxArcSteps*
:   Maximum number of arc steps

*DArcLengthMultiplier*
:   Initial arc length multiplier

Gets the arc-length completion options for this nonlinear study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetArcLengthCompletionOptions( _    ByRef DMaxLoad As System.Double, _    ByRef DMaxDisplacement As System.Double, _    ByRef NUnit As System.Integer, _    ByRef NMaxArcSteps As System.Integer, _    ByRef DArcLengthMultiplier As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWNonLinearStudyOptions Dim DMaxLoad As System.Double Dim DMaxDisplacement As System.Double Dim NUnit As System.Integer Dim NMaxArcSteps As System.Integer Dim DArcLengthMultiplier As System.Double   instance.GetArcLengthCompletionOptions(DMaxLoad, DMaxDisplacement, NUnit, NMaxArcSteps, DArcLengthMultiplier) ``` | |

| C# |  |
| --- | --- |
| ``` void GetArcLengthCompletionOptions(     out System.double DMaxLoad,    out System.double DMaxDisplacement,    out System.int NUnit,    out System.int NMaxArcSteps,    out System.double DArcLengthMultiplier ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetArcLengthCompletionOptions(  &   [Out] System.double DMaxLoad, &   [Out] System.double DMaxDisplacement, &   [Out] System.int NUnit, &   [Out] System.int NMaxArcSteps, &   [Out] System.double DArcLengthMultiplier ) ``` | |

#### Parameters

*DMaxLoad*
:   Maximum load-pattern multiplier

*DMaxDisplacement*
:   Maximum displacement (for translational DOF)

*NUnit*
:   Units as defined in [swsLinearUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinearUnit_e.html)

*NMaxArcSteps*
:   Maximum number of arc steps

*DArcLengthMultiplier*
:   Initial arc length multiplier

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWNonLinearStudyOptions::GetArcLengthCompletionOptions.

# ![](dotnetimages/collapse.gif)Example

See the [ICWNonLinearStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html)

[ICWNonLinearStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions_members.html)

[ICWNonLinaerStudyOptions::SetArcLengthCompletionOptions Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~SetArcLengthCompletionOptions.html)

[ICWNonLinaerStudyOptions::ControlMethodType Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~ControlMethodType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2010 SP3.0