<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~SetReverseDirections2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetReverseDirections2 Method (ICWRestraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html) : SetReverseDirections2 Method (ICWRestraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BVal1*
:   -1 or true to reverse plane direction 1, 0 or false to not; valid only if BVal1 of [ICWRestraint::GetTranslationComponentsValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetTranslationComponentsValues2.html) is set to -1 or true (see **Remarks**)

*BVal2*
:   -1 or true to reverse plane direction 2, 0 or false to not; valid only if BVal2 of ICWRestraint::GetTranslationComponentsValues2 is set to -1 or true (see **Remarks**)

*BVal3*
:   -1 or true to reverse the normal to the plane, 0 or false to not; valid only if BVal3 of ICWRestraint::GetTranslationComponentsValues2 is set to -1 or true (see **Remarks**)

*BVal4*
:   -1 or true to reverse radial direction, 0 or false to not; valid only if BVal1 of [ICWRestraint::GetRotationComponentsValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetRotationComponentsValues2.html) is set to -1 or true (see **Remarks**)

*BVal5*
:   -1 or true to reverse circumferential direction, 0 or false to not; valid only if BVal2 of ICWRestraint::GetRotationComponentsValues2 is set to -1 or true (see **Remarks**)

*BVal6*
:   -1 or true to reverse axial direction, 0 or false to not; valid only if BVal3 of ICWRestraint::GetRotationComponentsValues2 is set to -1 or true (see **Remarks**)

Sets whether to reverse the translation and rotation component directions for this restraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetReverseDirections2( _    ByVal BVal1 As System.Boolean, _    ByVal BVal2 As System.Boolean, _    ByVal BVal3 As System.Boolean, _    ByVal BVal4 As System.Boolean, _    ByVal BVal5 As System.Boolean, _    ByVal BVal6 As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRestraint Dim BVal1 As System.Boolean Dim BVal2 As System.Boolean Dim BVal3 As System.Boolean Dim BVal4 As System.Boolean Dim BVal5 As System.Boolean Dim BVal6 As System.Boolean   instance.SetReverseDirections2(BVal1, BVal2, BVal3, BVal4, BVal5, BVal6) ``` | |

| C# |  |
| --- | --- |
| ``` void SetReverseDirections2(     System.bool BVal1,    System.bool BVal2,    System.bool BVal3,    System.bool BVal4,    System.bool BVal5,    System.bool BVal6 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetReverseDirections2(  &   System.bool BVal1, &   System.bool BVal2, &   System.bool BVal3, &   System.bool BVal4, &   System.bool BVal5, &   System.bool BVal6 ) ``` | |

#### Parameters

*BVal1*
:   -1 or true to reverse plane direction 1, 0 or false to not; valid only if BVal1 of [ICWRestraint::GetTranslationComponentsValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetTranslationComponentsValues2.html) is set to -1 or true (see **Remarks**)

*BVal2*
:   -1 or true to reverse plane direction 2, 0 or false to not; valid only if BVal2 of ICWRestraint::GetTranslationComponentsValues2 is set to -1 or true (see **Remarks**)

*BVal3*
:   -1 or true to reverse the normal to the plane, 0 or false to not; valid only if BVal3 of ICWRestraint::GetTranslationComponentsValues2 is set to -1 or true (see **Remarks**)

*BVal4*
:   -1 or true to reverse radial direction, 0 or false to not; valid only if BVal1 of [ICWRestraint::GetRotationComponentsValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetRotationComponentsValues2.html) is set to -1 or true (see **Remarks**)

*BVal5*
:   -1 or true to reverse circumferential direction, 0 or false to not; valid only if BVal2 of ICWRestraint::GetRotationComponentsValues2 is set to -1 or true (see **Remarks**)

*BVal6*
:   -1 or true to reverse axial direction, 0 or false to not; valid only if BVal3 of ICWRestraint::GetRotationComponentsValues2 is set to -1 or true (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRestraint::SetReverseDirections2.

# ![](dotnetimages/collapse.gif)Remarks

Specify booleans or integers in parameters BVal1-6: true = -1 and false = 0.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html)

[ICWRestraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2021 SP04