<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetReverseDirections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetReverseDirections Method (ICWRestraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html) : GetReverseDirections Method (ICWRestraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BVal1*
:   1 if plane direction 1 is reversed, 0 if not; valid only if BVal1 of [ICWRestraint::GetTranslationComponentsValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetTranslationComponentsValues.html) is set to 1

*BVal2*
:   1 if plane direction 2 is reversed, 0 if not; valid only if BVal2 of ICWRestraint::GetTranslationComponentsValues is set to 1

*BVal3*
:   1 if normal to the plane is reversed, 0 if not; valid only if BVal3 of ICWRestraint::GetTranslationComponentsValues is set to 1

*BVal4*
:   1 if radial direction is reversed, 0 if not; valid only if BVal1 of [ICWRestraint::GetRotationComponentsValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetRotationComponentsValues.html) is set to 1

*BVal5*
:   1 if circumferential direction is reversed, 0 if not; valid only if BVal2 of ICWRestraint::GetRotationComponentsValues is set to 1

*BVal6*
:   1 if axial direction is reversed, 0 if not; valid only if BVal3 of ICWRestraint::GetRotationComponentsValues is set to 1

Obsolete. Superseded by [ICWRestraint::GetReverseDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetReverseDirections2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetReverseDirections( _    ByRef BVal1 As System.Integer, _    ByRef BVal2 As System.Integer, _    ByRef BVal3 As System.Integer, _    ByRef BVal4 As System.Integer, _    ByRef BVal5 As System.Integer, _    ByRef BVal6 As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRestraint Dim BVal1 As System.Integer Dim BVal2 As System.Integer Dim BVal3 As System.Integer Dim BVal4 As System.Integer Dim BVal5 As System.Integer Dim BVal6 As System.Integer   instance.GetReverseDirections(BVal1, BVal2, BVal3, BVal4, BVal5, BVal6) ``` | |

| C# |  |
| --- | --- |
| ``` void GetReverseDirections(     out System.int BVal1,    out System.int BVal2,    out System.int BVal3,    out System.int BVal4,    out System.int BVal5,    out System.int BVal6 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetReverseDirections(  &   [Out] System.int BVal1, &   [Out] System.int BVal2, &   [Out] System.int BVal3, &   [Out] System.int BVal4, &   [Out] System.int BVal5, &   [Out] System.int BVal6 ) ``` | |

#### Parameters

*BVal1*
:   1 if plane direction 1 is reversed, 0 if not; valid only if BVal1 of [ICWRestraint::GetTranslationComponentsValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetTranslationComponentsValues.html) is set to 1

*BVal2*
:   1 if plane direction 2 is reversed, 0 if not; valid only if BVal2 of ICWRestraint::GetTranslationComponentsValues is set to 1

*BVal3*
:   1 if normal to the plane is reversed, 0 if not; valid only if BVal3 of ICWRestraint::GetTranslationComponentsValues is set to 1

*BVal4*
:   1 if radial direction is reversed, 0 if not; valid only if BVal1 of [ICWRestraint::GetRotationComponentsValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetRotationComponentsValues.html) is set to 1

*BVal5*
:   1 if circumferential direction is reversed, 0 if not; valid only if BVal2 of ICWRestraint::GetRotationComponentsValues is set to 1

*BVal6*
:   1 if axial direction is reversed, 0 if not; valid only if BVal3 of ICWRestraint::GetRotationComponentsValues is set to 1

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRestraint::GetReverseDirections.

# ![](dotnetimages/collapse.gif)Example

See the [ICWRestraint](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html)

[ICWRestraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint_members.html)

[ICWRestraint::SetReverseDirections Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~SetReverseDirections.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0