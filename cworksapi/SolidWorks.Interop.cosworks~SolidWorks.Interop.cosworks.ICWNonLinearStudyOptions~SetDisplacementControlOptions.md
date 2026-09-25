<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~SetDisplacementControlOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetDisplacementControlOptions Method (ICWNonLinearStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) : SetDisplacementControlOptions Method (ICWNonLinearStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispEntity*
:   Vertex or reference point to control the analysis

*NDisplacementComponent*
:   Displacement component for the selected location (see **Remarks**)

*NUnit*
:   Units as defined in [swsLinearUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinearUnit_e.html)

Sets displacement control options for this nonlinear study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetDisplacementControlOptions( _    ByVal DispEntity As System.Object, _    ByVal NDisplacementComponent As System.Integer, _    ByVal NUnit As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWNonLinearStudyOptions Dim DispEntity As System.Object Dim NDisplacementComponent As System.Integer Dim NUnit As System.Integer Dim value As System.Integer   value = instance.SetDisplacementControlOptions(DispEntity, NDisplacementComponent, NUnit) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetDisplacementControlOptions(     System.object DispEntity,    System.int NDisplacementComponent,    System.int NUnit ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetDisplacementControlOptions(  &   System.Object^ DispEntity, &   System.int NDisplacementComponent, &   System.int NUnit ) ``` | |

#### Parameters

*DispEntity*
:   Vertex or reference point to control the analysis

*NDisplacementComponent*
:   Displacement component for the selected location (see **Remarks**)

*NUnit*
:   Units as defined in [swsLinearUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinearUnit_e.html)

#### Return Value

Status as defined in [swsNonLinearStudyOptionsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNonLinearStudyOptionsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWNonLinearStudyOptions::SetDisplacementControlOptions.

# ![](dotnetimages/collapse.gif)Remarks

[ICWNonLinearStudyOptions::ControlMethodType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~ControlMethodType.html) must be set to [swsNonLinearOptionControlMethodType\_e.swsNonLinearControl\_Displacement](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNonLinearOptionControlMethodType_e.html) to set displacement control options.

Valid displacement components are:

UX: X Translation. displacement in the Global X-direction

UY: Y Translation. displacement in the Global Y-direction

UZ: Z Translation. displacement in the Global Z-direction

RX: X Rotation. rotation about the Global X-direction for shell studies only

RY: Y Rotation. rotation about the Global Y-direction for shell studies only

RZ: Z Rotation. rotation about the Global Z-direction for shell studies only

# ![](dotnetimages/collapse.gif)See Also

####

[ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html)

[ICWNonLinearStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions_members.html)

[ICWNonLinearStudyOptions::GetDisplacementControlOptions Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~GetDisplacementControlOptions.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2010 SP3.0