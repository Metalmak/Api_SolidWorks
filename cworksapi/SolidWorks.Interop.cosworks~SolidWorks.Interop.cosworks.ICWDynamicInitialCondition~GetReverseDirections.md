<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetReverseDirections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetReverseDirections Method (ICWDynamicInitialCondition) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicInitialCondition Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition.html) : GetReverseDirections Method (ICWDynamicInitialCondition) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BVal1*
:   1 if BDir1 of [ICWDynamicInitialCondition::GetDirections](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetDirections.html) is reversed, 0 if not

*BVal2*
:   1 if BDir2 of ICWDynamicInitialCondition::GetDirections is reversed, 0 if not

*BVal3*
:   1 if BDir3 of ICWDynamicInitialCondition::GetDirections is reversed, 0 if not

Obsolete. Superseded by [ICWDynamicInitialCondition::GetReverseDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetReverseDirections2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetReverseDirections( _    ByRef BVal1 As System.Integer, _    ByRef BVal2 As System.Integer, _    ByRef BVal3 As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicInitialCondition Dim BVal1 As System.Integer Dim BVal2 As System.Integer Dim BVal3 As System.Integer   instance.GetReverseDirections(BVal1, BVal2, BVal3) ``` | |

| C# |  |
| --- | --- |
| ``` void GetReverseDirections(     out System.int BVal1,    out System.int BVal2,    out System.int BVal3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetReverseDirections(  &   [Out] System.int BVal1, &   [Out] System.int BVal2, &   [Out] System.int BVal3 ) ``` | |

#### Parameters

*BVal1*
:   1 if BDir1 of [ICWDynamicInitialCondition::GetDirections](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetDirections.html) is reversed, 0 if not

*BVal2*
:   1 if BDir2 of ICWDynamicInitialCondition::GetDirections is reversed, 0 if not

*BVal3*
:   1 if BDir3 of ICWDynamicInitialCondition::GetDirections is reversed, 0 if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDynamicInitialCondition::GetReverseDirections.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicInitialCondition Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition.html)

[ICWDynamicInitialCondition Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition_members.html)

[ICWDynamicInitialCondition::SetReverseDirections Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetReverseDirections.html)

[ICWDynamicInitialCondition::SetDirectionEntity Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetDirectionEntity.html)

[ICWDynamicInitialCondition::GetValues Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0