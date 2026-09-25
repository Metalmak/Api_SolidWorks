<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~GetSaveStressAndReactionsOptions2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetSaveStressAndReactionsOptions2 Method (ICWStudyResultOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html) : GetSaveStressAndReactionsOptions2 Method (ICWStudyResultOptions) |

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
:   -1 or true to save nodal von Mises stresses only, 0 to save all stress components; valid only if BSaveStressAndReactions is set to -1

Gets whether to save stress and reaction results and, if so, whether to save them for all stress components or nodal von Mises stresses only.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSaveStressAndReactionsOptions2( _    ByRef BSaveStressAndReactions As System.Boolean, _    ByRef BVonMisesOnly As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyResultOptions Dim BSaveStressAndReactions As System.Boolean Dim BVonMisesOnly As System.Boolean Dim value As System.Boolean   value = instance.GetSaveStressAndReactionsOptions2(BSaveStressAndReactions, BVonMisesOnly) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetSaveStressAndReactionsOptions2(     out System.bool BSaveStressAndReactions,    out System.bool BVonMisesOnly ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetSaveStressAndReactionsOptions2(  &   [Out] System.bool BSaveStressAndReactions, &   [Out] System.bool BVonMisesOnly ) ``` | |

#### Parameters

*BSaveStressAndReactions*
:   -1 or true to save stress and reaction results, 0 or false to not

*BVonMisesOnly*
:   -1 or true to save nodal von Mises stresses only, 0 to save all stress components; valid only if BSaveStressAndReactions is set to -1

#### Return Value

-1 or true if successful, 0 or false if not

# ![](dotnetimages/collapse.gif)Remarks

This method returns booleans or integers in the out parameters, depending on their prior declarations.

If out parameters are cast as:

* Booleans, true or false is returned in each out parameter.* Longs or integers, -1 (=true) or 0 (=false) is returned in each out parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html)

[ICWStudyResultOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30