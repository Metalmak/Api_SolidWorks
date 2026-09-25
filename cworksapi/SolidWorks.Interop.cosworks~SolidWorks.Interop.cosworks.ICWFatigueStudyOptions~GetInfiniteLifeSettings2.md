<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions~GetInfiniteLifeSettings2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetInfiniteLifeSettings2 Method (ICWFatigueStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWFatigueStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions.html) : GetInfiniteLifeSettings2 Method (ICWFatigueStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BChecked*
:   -1 or true to use DCyles number of cycles; 0 or false to use the number of cycles associated with the last point of an S-N curve

*DCycles*
:   Number of cycles to use when the corrected alternating stress is less than the endurance limit; valid only if BChecked is -1

Gets the infinite life settings of the fatigue study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetInfiniteLifeSettings2( _    ByRef BChecked As System.Boolean, _    ByRef DCycles As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWFatigueStudyOptions Dim BChecked As System.Boolean Dim DCycles As System.Double   instance.GetInfiniteLifeSettings2(BChecked, DCycles) ``` | |

| C# |  |
| --- | --- |
| ``` void GetInfiniteLifeSettings2(     out System.bool BChecked,    out System.double DCycles ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetInfiniteLifeSettings2(  &   [Out] System.bool BChecked, &   [Out] System.double DCycles ) ``` | |

#### Parameters

*BChecked*
:   -1 or true to use DCyles number of cycles; 0 or false to use the number of cycles associated with the last point of an S-N curve

*DCycles*
:   Number of cycles to use when the corrected alternating stress is less than the endurance limit; valid only if BChecked is -1

# ![](dotnetimages/collapse.gif)Example

See the [ICWFatigueStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWFatigueStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions.html)

[ICWFatigueStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30