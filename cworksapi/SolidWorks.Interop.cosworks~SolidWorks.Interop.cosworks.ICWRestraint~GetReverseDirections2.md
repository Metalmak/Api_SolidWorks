<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetReverseDirections2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetReverseDirections2 Method (ICWRestraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html) : GetReverseDirections2 Method (ICWRestraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BVal1*
:   -1 or true if plane direction 1 is reversed, 0 or false if not; valid only if BVal1 of [ICWRestraint::GetTranslationComponentsValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetTranslationComponentsValues2.html) is set to -1 or true (see **Remarks**)

*BVal2*
:   -1 or true if plane direction 2 is reversed, 0 or false if not; valid only if BVal2 of ICWRestraint::GetTranslationComponentsValues2 is set to -1 or true (see **Remarks**)

*BVal3*
:   -1 or true if normal to the plane is reversed, 0 or false if not; valid only if BVal3 of ICWRestraint::GetTranslationComponentsValues2 is set to -1 or true (see **Remarks**)

*BVal4*
:   -1 or true if radial direction is reversed, 0 or false if not; valid only if BVal1 of [ICWRestraint::GetRotationComponentsValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetRotationComponentsValues2.html) is set to -1 or true (see **Remarks**)

*BVal5*
:   -1 or true if circumferential direction is reversed, 0 or false if not; valid only if BVal2 of ICWRestraint::GetRotationComponentsValues2 is set to -1 or true (see **Remarks**)

*BVal6*
:   -1 or true if axial direction is reversed, 0 or false if not; valid only if BVal3 of ICWRestraint::GetRotationComponentsValues2 is set to -1 or true (see **Remarks**)

Gets whether to reverse the translation and rotation component directions for this restraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetReverseDirections2( _    ByRef BVal1 As System.Boolean, _    ByRef BVal2 As System.Boolean, _    ByRef BVal3 As System.Boolean, _    ByRef BVal4 As System.Boolean, _    ByRef BVal5 As System.Boolean, _    ByRef BVal6 As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRestraint Dim BVal1 As System.Boolean Dim BVal2 As System.Boolean Dim BVal3 As System.Boolean Dim BVal4 As System.Boolean Dim BVal5 As System.Boolean Dim BVal6 As System.Boolean   instance.GetReverseDirections2(BVal1, BVal2, BVal3, BVal4, BVal5, BVal6) ``` | |

| C# |  |
| --- | --- |
| ``` void GetReverseDirections2(     out System.bool BVal1,    out System.bool BVal2,    out System.bool BVal3,    out System.bool BVal4,    out System.bool BVal5,    out System.bool BVal6 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetReverseDirections2(  &   [Out] System.bool BVal1, &   [Out] System.bool BVal2, &   [Out] System.bool BVal3, &   [Out] System.bool BVal4, &   [Out] System.bool BVal5, &   [Out] System.bool BVal6 ) ``` | |

#### Parameters

*BVal1*
:   -1 or true if plane direction 1 is reversed, 0 or false if not; valid only if BVal1 of [ICWRestraint::GetTranslationComponentsValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetTranslationComponentsValues2.html) is set to -1 or true (see **Remarks**)

*BVal2*
:   -1 or true if plane direction 2 is reversed, 0 or false if not; valid only if BVal2 of ICWRestraint::GetTranslationComponentsValues2 is set to -1 or true (see **Remarks**)

*BVal3*
:   -1 or true if normal to the plane is reversed, 0 or false if not; valid only if BVal3 of ICWRestraint::GetTranslationComponentsValues2 is set to -1 or true (see **Remarks**)

*BVal4*
:   -1 or true if radial direction is reversed, 0 or false if not; valid only if BVal1 of [ICWRestraint::GetRotationComponentsValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetRotationComponentsValues2.html) is set to -1 or true (see **Remarks**)

*BVal5*
:   -1 or true if circumferential direction is reversed, 0 or false if not; valid only if BVal2 of ICWRestraint::GetRotationComponentsValues2 is set to -1 or true (see **Remarks**)

*BVal6*
:   -1 or true if axial direction is reversed, 0 or false if not; valid only if BVal3 of ICWRestraint::GetRotationComponentsValues2 is set to -1 or true (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRestraint::GetReverseDirections2.

# ![](dotnetimages/collapse.gif)Remarks

This method returns booleans or integers in out parameters BVal1-6, depending on their prior declarations.

If out parameters BVal1-6 are cast as:

* Booleans, true or false is returned in each out parameter.* Longs or integers, -1 (=true) or 0 (=false) is returned in each out parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html)

[ICWRestraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2021 SP04