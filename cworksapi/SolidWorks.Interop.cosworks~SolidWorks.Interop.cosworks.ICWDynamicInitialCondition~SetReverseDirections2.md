<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetReverseDirections2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetReverseDirections2 Method (ICWDynamicInitialCondition) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicInitialCondition Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition.html) : SetReverseDirections2 Method (ICWDynamicInitialCondition) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BVal1*
:   -1 or true to reverse BDir1 of [ICWDynamicInitialCondition::GetDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetDirections2.html), 0 or false to not

*BVal2*
:   -1 or true to reverse BDir2 of ICWDynamicInitialCondition::GetDirections2, 0 or false to not

*BVal3*
:   -1 or true to reverse BDir3 of ICWDynamicInitialCondition::GetDirections2, 0 or false to not

Sets whether the directions of this initial condition are reversed.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetReverseDirections2( _    ByVal BVal1 As System.Boolean, _    ByVal BVal2 As System.Boolean, _    ByVal BVal3 As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicInitialCondition Dim BVal1 As System.Boolean Dim BVal2 As System.Boolean Dim BVal3 As System.Boolean   instance.SetReverseDirections2(BVal1, BVal2, BVal3) ``` | |

| C# |  |
| --- | --- |
| ``` void SetReverseDirections2(     System.bool BVal1,    System.bool BVal2,    System.bool BVal3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetReverseDirections2(  &   System.bool BVal1, &   System.bool BVal2, &   System.bool BVal3 ) ``` | |

#### Parameters

*BVal1*
:   -1 or true to reverse BDir1 of [ICWDynamicInitialCondition::GetDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetDirections2.html), 0 or false to not

*BVal2*
:   -1 or true to reverse BDir2 of ICWDynamicInitialCondition::GetDirections2, 0 or false to not

*BVal3*
:   -1 or true to reverse BDir3 of ICWDynamicInitialCondition::GetDirections2, 0 or false to not

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicInitialCondition Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition.html)

[ICWDynamicInitialCondition Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30