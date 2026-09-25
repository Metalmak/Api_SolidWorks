<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent~SetStudyAssociationData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetStudyAssociationData Method (ICWFatigueEvent) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWFatigueEvent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent.html) : SetStudyAssociationData Method (ICWFatigueEvent) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NCount*
:   Number of study associations

*VarStudyNames*
:   Array of reference study names

*VarScales*
:   Array of scale factors to apply to the scaled loads of studies in VarStudyNames to calculate the alternating stresses; valid only if VarStudyNames contains the names of linear studies

*VarSteps*
:   Array of solution steps whose stress results are used to calculate the alternating stresses; valid only if VarStudyNames contains the names of nonlinear or linear dynamic studies

Sets the study association data for this fatigue event.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetStudyAssociationData( _    ByVal NCount As System.Integer, _    ByVal VarStudyNames As System.Object, _    ByVal VarScales As System.Object, _    ByVal VarSteps As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWFatigueEvent Dim NCount As System.Integer Dim VarStudyNames As System.Object Dim VarScales As System.Object Dim VarSteps As System.Object Dim value As System.Integer   value = instance.SetStudyAssociationData(NCount, VarStudyNames, VarScales, VarSteps) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetStudyAssociationData(     System.int NCount,    System.object VarStudyNames,    System.object VarScales,    System.object VarSteps ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetStudyAssociationData(  &   System.int NCount, &   System.Object^ VarStudyNames, &   System.Object^ VarScales, &   System.Object^ VarSteps ) ``` | |

#### Parameters

*NCount*
:   Number of study associations

*VarStudyNames*
:   Array of reference study names

*VarScales*
:   Array of scale factors to apply to the scaled loads of studies in VarStudyNames to calculate the alternating stresses; valid only if VarStudyNames contains the names of linear studies

*VarSteps*
:   Array of solution steps whose stress results are used to calculate the alternating stresses; valid only if VarStudyNames contains the names of nonlinear or linear dynamic studies

#### Return Value

Error code as defined in [swsFatigueEventEndEditError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueEventEndEditError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWFatigueEvent::SetStudyAssociationData.

# ![](dotnetimages/collapse.gif)Example

See the [ICWFatigueEvent](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWFatigueEvent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent.html)

[ICWFatigueEvent Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent_members.html)

[ICWFatigueEvent::GetStudyAssociationData Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent~GetStudyAssociationData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0