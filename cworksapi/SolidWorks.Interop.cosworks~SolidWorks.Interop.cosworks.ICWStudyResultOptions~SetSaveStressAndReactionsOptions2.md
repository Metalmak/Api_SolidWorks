<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SetSaveStressAndReactionsOptions2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetSaveStressAndReactionsOptions2 Method (ICWStudyResultOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html) : SetSaveStressAndReactionsOptions2 Method (ICWStudyResultOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BSaveStressAndReactions*
:   -1 or true to save stress and reaction results, 0 or false to not

*BVonMisesOnly*
:   -1 or true to save nodal von Mises stresses only, 0 or false to save all stress components; valid only if BSaveStressAndReactions is set to -1

Sets whether to save stress and reaction results and, if so, whether to save them for all stress components or nodal von Mises stresses only.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSaveStressAndReactionsOptions2( _    ByVal BSaveStressAndReactions As System.Boolean, _    ByVal BVonMisesOnly As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyResultOptions Dim BSaveStressAndReactions As System.Boolean Dim BVonMisesOnly As System.Boolean Dim value As System.Boolean   value = instance.SetSaveStressAndReactionsOptions2(BSaveStressAndReactions, BVonMisesOnly) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSaveStressAndReactionsOptions2(     System.bool BSaveStressAndReactions,    System.bool BVonMisesOnly ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSaveStressAndReactionsOptions2(  &   System.bool BSaveStressAndReactions, &   System.bool BVonMisesOnly ) ``` | |

#### Parameters

*BSaveStressAndReactions*
:   -1 or true to save stress and reaction results, 0 or false to not

*BVonMisesOnly*
:   -1 or true to save nodal von Mises stresses only, 0 or false to save all stress components; valid only if BSaveStressAndReactions is set to -1

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Example

See the [ICWStudyResultOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html)

[ICWStudyResultOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30