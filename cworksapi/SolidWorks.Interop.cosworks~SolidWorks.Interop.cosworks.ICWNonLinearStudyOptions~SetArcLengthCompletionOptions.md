<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~SetArcLengthCompletionOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetArcLengthCompletionOptions Method (ICWNonLinearStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) : SetArcLengthCompletionOptions Method (ICWNonLinearStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DMaxLoad*
:   Maximum load pattern multiplier

*DMaxDisplacement*
:   Maximum displacement (for translational DOF)

*NUnit*
:   Units as defined in [swsLinearUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinearUnit_e.html)

*NArcSteps*
:   Maximum number of arc steps

*DArcLenMultiplier*
:   Initial arc length multiplier

Sets arc-length completion options for this nonlinear study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetArcLengthCompletionOptions( _    ByVal DMaxLoad As System.Double, _    ByVal DMaxDisplacement As System.Double, _    ByVal NUnit As System.Integer, _    ByVal NArcSteps As System.Integer, _    ByVal DArcLenMultiplier As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWNonLinearStudyOptions Dim DMaxLoad As System.Double Dim DMaxDisplacement As System.Double Dim NUnit As System.Integer Dim NArcSteps As System.Integer Dim DArcLenMultiplier As System.Double Dim value As System.Integer   value = instance.SetArcLengthCompletionOptions(DMaxLoad, DMaxDisplacement, NUnit, NArcSteps, DArcLenMultiplier) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetArcLengthCompletionOptions(     System.double DMaxLoad,    System.double DMaxDisplacement,    System.int NUnit,    System.int NArcSteps,    System.double DArcLenMultiplier ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetArcLengthCompletionOptions(  &   System.double DMaxLoad, &   System.double DMaxDisplacement, &   System.int NUnit, &   System.int NArcSteps, &   System.double DArcLenMultiplier ) ``` | |

#### Parameters

*DMaxLoad*
:   Maximum load pattern multiplier

*DMaxDisplacement*
:   Maximum displacement (for translational DOF)

*NUnit*
:   Units as defined in [swsLinearUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinearUnit_e.html)

*NArcSteps*
:   Maximum number of arc steps

*DArcLenMultiplier*
:   Initial arc length multiplier

#### Return Value

Status as defined in [swsNonLinearStudyOptionsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNonLinearStudyOptionsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWNonLinearStudyOptions::SetArcLengthCompletionOptions.

# ![](dotnetimages/collapse.gif)Remarks

[ICWNonLinearStudyOptions::ControlMethodType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~ControlMethodType.html) must be set to [swsNonLinearOptionControlMethodType\_e.swsNonLinearControl\_ArcLength](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNonLinearOptionControlMethodType_e.html) to set arc-length completion options.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html)

[ICWNonLinearStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions_members.html)

[ICWNonLinearStudyOptions::GetArcLengthCompletionOptions Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~GetArcLengthCompletionOptions.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2010 SP3.0