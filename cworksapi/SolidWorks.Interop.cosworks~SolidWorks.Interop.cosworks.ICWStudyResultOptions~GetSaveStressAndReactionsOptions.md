<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~GetSaveStressAndReactionsOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetSaveStressAndReactionsOptions Method (ICWStudyResultOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html) : GetSaveStressAndReactionsOptions Method (ICWStudyResultOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BSaveStressAndReactions*
:   1 to save stress and reaction results, 0 to not

*BVonMisesOnly*
:   1 to save nodal von Mises stresses only, 0 to save all stress components; valid only if BSaveStressAndReactions is set to 1

Obsolete. Superseded by [ICWStudyResultOptions::GetSaveStressAndReactionsOptions2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~GetSaveStressAndReactionsOptions2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSaveStressAndReactionsOptions( _    ByRef BSaveStressAndReactions As System.Integer, _    ByRef BVonMisesOnly As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyResultOptions Dim BSaveStressAndReactions As System.Integer Dim BVonMisesOnly As System.Integer Dim value As System.Boolean   value = instance.GetSaveStressAndReactionsOptions(BSaveStressAndReactions, BVonMisesOnly) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetSaveStressAndReactionsOptions(     out System.int BSaveStressAndReactions,    out System.int BVonMisesOnly ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetSaveStressAndReactionsOptions(  &   [Out] System.int BSaveStressAndReactions, &   [Out] System.int BVonMisesOnly ) ``` | |

#### Parameters

*BSaveStressAndReactions*
:   1 to save stress and reaction results, 0 to not

*BVonMisesOnly*
:   1 to save nodal von Mises stresses only, 0 to save all stress components; valid only if BSaveStressAndReactions is set to 1

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyResultOptions::GetSaveStressAndReactionsOptions.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html)

[ICWStudyResultOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions_members.html)

[ICWStudyResultOptions::SetSaveStressAndReactionsOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SetSaveStressAndReactionsOptions.html)

[ICWStudyResultOptions::SaveDisplacementsAndVelocitiesOption Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SaveDisplacementsAndVelocitiesOption.html)

[ICWStudyResultOptions::SaveResultsForSolutionStepsOption Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SaveResultsForSolutionStepsOption.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0