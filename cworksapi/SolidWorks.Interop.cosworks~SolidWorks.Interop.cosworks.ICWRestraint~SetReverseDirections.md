<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~SetReverseDirections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetReverseDirections Method (ICWRestraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html) : SetReverseDirections Method (ICWRestraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BVal1*
:   1 to reverse plane direction 1, 0 to not; valid only if BVal1 of [ICWRestraint::GetTranslationComponentsValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetTranslationComponentsValues.html) is set to 1

*BVal2*
:   1 to reverse plane direction 2, 0 to not; valid only if BVal2 of ICWRestraint::GetTranslationComponentsValues is set to 1

*BVal3*
:   1 to reverse the normal to the plane, 0 to not; valid only if BVal3 of ICWRestraint::GetTranslationComponentsValues is set to 1

*BVal4*
:   1 to reverse radial direction, 0 to not; valid only if BVal1 of [ICWRestraint::GetRotationComponentsValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetRotationComponentsValues.html) is set to 1

*BVal5*
:   1 to reverse circumferential direction, 0 to not; valid only if BVal2 of ICWRestraint::GetRotationComponentsValues is set to 1

*BVal6*
:   1 to reverse axial direction, 0 to not; valid only if BVal3 of ICWRestraint::GetRotationComponentsValues is set to 1

Obsolete. Superseded by [ICWRestraint::SetReverseDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~SetReverseDirections2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetReverseDirections( _    ByVal BVal1 As System.Integer, _    ByVal BVal2 As System.Integer, _    ByVal BVal3 As System.Integer, _    ByVal BVal4 As System.Integer, _    ByVal BVal5 As System.Integer, _    ByVal BVal6 As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRestraint Dim BVal1 As System.Integer Dim BVal2 As System.Integer Dim BVal3 As System.Integer Dim BVal4 As System.Integer Dim BVal5 As System.Integer Dim BVal6 As System.Integer   instance.SetReverseDirections(BVal1, BVal2, BVal3, BVal4, BVal5, BVal6) ``` | |

| C# |  |
| --- | --- |
| ``` void SetReverseDirections(     System.int BVal1,    System.int BVal2,    System.int BVal3,    System.int BVal4,    System.int BVal5,    System.int BVal6 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetReverseDirections(  &   System.int BVal1, &   System.int BVal2, &   System.int BVal3, &   System.int BVal4, &   System.int BVal5, &   System.int BVal6 ) ``` | |

#### Parameters

*BVal1*
:   1 to reverse plane direction 1, 0 to not; valid only if BVal1 of [ICWRestraint::GetTranslationComponentsValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetTranslationComponentsValues.html) is set to 1

*BVal2*
:   1 to reverse plane direction 2, 0 to not; valid only if BVal2 of ICWRestraint::GetTranslationComponentsValues is set to 1

*BVal3*
:   1 to reverse the normal to the plane, 0 to not; valid only if BVal3 of ICWRestraint::GetTranslationComponentsValues is set to 1

*BVal4*
:   1 to reverse radial direction, 0 to not; valid only if BVal1 of [ICWRestraint::GetRotationComponentsValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetRotationComponentsValues.html) is set to 1

*BVal5*
:   1 to reverse circumferential direction, 0 to not; valid only if BVal2 of ICWRestraint::GetRotationComponentsValues is set to 1

*BVal6*
:   1 to reverse axial direction, 0 to not; valid only if BVal3 of ICWRestraint::GetRotationComponentsValues is set to 1

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRestraint::SetReverseDirections.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html)

[ICWRestraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint_members.html)

[ICWRestraint::GetReverseDirections Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetReverseDirections.html)

[ICWRestraint::SetRotationComponentsValues Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~SetRotationComponentsValues.html)

[ICWRestraint::SetTranslationComponentsValues Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~SetTranslationComponentsValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0