<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent~GetStudyAssociationData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetStudyAssociationData Method (ICWFatigueEvent) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWFatigueEvent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent.html) : GetStudyAssociationData Method (ICWFatigueEvent) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VarStudyNames*
:   Array of reference study names

*VarScales*
:   Array of scale factors to apply to the scaled loads of studies in VarStudyNames to calculate the alternating stresses; valid only if VarStudyNames contains the names of linear studies

*VarSteps*
:   Array of solution steps whose stress results are used to calculate the alternating stresses; valid only if VarStudyNames contains the names of nonlinear or linear dynamic studies

Gets the study association data for this fatigue event.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetStudyAssociationData( _    ByRef VarStudyNames As System.Object, _    ByRef VarScales As System.Object, _    ByRef VarSteps As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWFatigueEvent Dim VarStudyNames As System.Object Dim VarScales As System.Object Dim VarSteps As System.Object Dim value As System.Integer   value = instance.GetStudyAssociationData(VarStudyNames, VarScales, VarSteps) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetStudyAssociationData(     out System.object VarStudyNames,    out System.object VarScales,    out System.object VarSteps ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetStudyAssociationData(  &   [Out] System.Object^ VarStudyNames, &   [Out] System.Object^ VarScales, &   [Out] System.Object^ VarSteps ) ``` | |

#### Parameters

*VarStudyNames*
:   Array of reference study names

*VarScales*
:   Array of scale factors to apply to the scaled loads of studies in VarStudyNames to calculate the alternating stresses; valid only if VarStudyNames contains the names of linear studies

*VarSteps*
:   Array of solution steps whose stress results are used to calculate the alternating stresses; valid only if VarStudyNames contains the names of nonlinear or linear dynamic studies

#### Return Value

Number of study associations

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWFatigueEvent::GetStudyAssociationData.

# ![](dotnetimages/collapse.gif)Example

See the [ICWFatigueEvent](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWFatigueEvent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent.html)

[ICWFatigueEvent Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent_members.html)

[ICWFatigueEvent::SetStudyAssociationData Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent~SetStudyAssociationData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0