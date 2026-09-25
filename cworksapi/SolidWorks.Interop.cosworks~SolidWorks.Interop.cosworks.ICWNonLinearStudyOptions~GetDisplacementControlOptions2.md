<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~GetDisplacementControlOptions2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetDisplacementControlOptions2 Method (ICWNonLinearStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) : GetDisplacementControlOptions2 Method (ICWNonLinearStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NDisplacementComponent*
:   Displacement component for the selected location

*NUnit*
:   Unit as defined in [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*Dispatch*
:   Selected vertex or reference point to control the analysis

Gets displacement control options for this nonlinear study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetDisplacementControlOptions2( _    ByRef NDisplacementComponent As System.Integer, _    ByRef NUnit As System.Integer, _    ByRef Dispatch As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWNonLinearStudyOptions Dim NDisplacementComponent As System.Integer Dim NUnit As System.Integer Dim Dispatch As System.Object   instance.GetDisplacementControlOptions2(NDisplacementComponent, NUnit, Dispatch) ``` | |

| C# |  |
| --- | --- |
| ``` void GetDisplacementControlOptions2(     out System.int NDisplacementComponent,    out System.int NUnit,    out System.object Dispatch ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetDisplacementControlOptions2(  &   [Out] System.int NDisplacementComponent, &   [Out] System.int NUnit, &   [Out] System.Object^ Dispatch ) ``` | |

#### Parameters

*NDisplacementComponent*
:   Displacement component for the selected location

*NUnit*
:   Unit as defined in [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*Dispatch*
:   Selected vertex or reference point to control the analysis

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWNonLinearStudyOptions::GetDisplacementControlOptions2.

# ![](dotnetimages/collapse.gif)Example

See the [ICWNonLinearStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html)

[ICWNonLinearStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions_members.html)

[ICWNonLinearStudyOptions::SetDisplacementControlOptions Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~SetDisplacementControlOptions.html)

[ICWNonLinearStudyOptions::ControlMethodType Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~ControlMethodType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2010 SP5.0 and SOLIDWORKS Simulation 2011 SP1.0