<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetReverseDirections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetReverseDirections Method (ICWDynamicInitialCondition) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicInitialCondition Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition.html) : SetReverseDirections Method (ICWDynamicInitialCondition) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BVal1*
:   1 to reverse BDir1 of [ICWDynamicInitialCondition::GetDirections](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetDirections.html), 0 to not

*BVal2*
:   1 to reverse BDir2 of ICWDynamicInitialCondition::GetDirections, 0 to not

*BVal3*
:   1 to reverse BDir3 of ICWDynamicInitialCondition::GetDirections, 0 to not

Obsolete. Superseded by [ICWDynamicInitialCondition::SetReverseDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetReverseDirections.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetReverseDirections( _    ByVal BVal1 As System.Integer, _    ByVal BVal2 As System.Integer, _    ByVal BVal3 As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicInitialCondition Dim BVal1 As System.Integer Dim BVal2 As System.Integer Dim BVal3 As System.Integer   instance.SetReverseDirections(BVal1, BVal2, BVal3) ``` | |

| C# |  |
| --- | --- |
| ``` void SetReverseDirections(     System.int BVal1,    System.int BVal2,    System.int BVal3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetReverseDirections(  &   System.int BVal1, &   System.int BVal2, &   System.int BVal3 ) ``` | |

#### Parameters

*BVal1*
:   1 to reverse BDir1 of [ICWDynamicInitialCondition::GetDirections](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetDirections.html), 0 to not

*BVal2*
:   1 to reverse BDir2 of ICWDynamicInitialCondition::GetDirections, 0 to not

*BVal3*
:   1 to reverse BDir3 of ICWDynamicInitialCondition::GetDirections, 0 to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDynamicInitialCondition::SetReverseDirections.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicInitialCondition Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition.html)

[ICWDynamicInitialCondition Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition_members.html)

[ICWDynamicInitialCondition::GetReverseDirections Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetReverseDirections.html)

[ICWDynamicInitialCondition::SetDirectionEntity Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetDirectionEntity.html)

[ICWDynamicInitialCondition::SetDirections Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetDirections.html)

[ICWDynamicInitialCondition::SetValues Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0