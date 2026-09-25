<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetRotationComponentsValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetRotationComponentsValues Method (ICWRestraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html) : GetRotationComponentsValues Method (ICWRestraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BVal1*
:   1 to use DVal1 , 0 to not

*BVal2*
:   1 to use DVal2, 0 to not

*BVal3*
:   1 to use DVal3, 0 to not

*DVal1*
:   (see **Remarks**)

*DVal2*
:   (see **Remarks**)

*DVal3*
:   (see **Remarks**)

Obsolete. Superseded by [ICWRestraint::GetRotationComponentsValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetRotationComponentsValues2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetRotationComponentsValues( _    ByRef BVal1 As System.Integer, _    ByRef BVal2 As System.Integer, _    ByRef BVal3 As System.Integer, _    ByRef DVal1 As System.Double, _    ByRef DVal2 As System.Double, _    ByRef DVal3 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRestraint Dim BVal1 As System.Integer Dim BVal2 As System.Integer Dim BVal3 As System.Integer Dim DVal1 As System.Double Dim DVal2 As System.Double Dim DVal3 As System.Double   instance.GetRotationComponentsValues(BVal1, BVal2, BVal3, DVal1, DVal2, DVal3) ``` | |

| C# |  |
| --- | --- |
| ``` void GetRotationComponentsValues(     out System.int BVal1,    out System.int BVal2,    out System.int BVal3,    out System.double DVal1,    out System.double DVal2,    out System.double DVal3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetRotationComponentsValues(  &   [Out] System.int BVal1, &   [Out] System.int BVal2, &   [Out] System.int BVal3, &   [Out] System.double DVal1, &   [Out] System.double DVal2, &   [Out] System.double DVal3 ) ``` | |

#### Parameters

*BVal1*
:   1 to use DVal1 , 0 to not

*BVal2*
:   1 to use DVal2, 0 to not

*BVal3*
:   1 to use DVal3, 0 to not

*DVal1*
:   (see **Remarks**)

*DVal2*
:   (see **Remarks**)

*DVal3*
:   (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRestraint::GetRotationComponentsValues.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for beams and shell meshes with [ICWRestraint::RestraintType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~RestraintType.html) set to:

* [swsRestraintType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRestraintType_e.html).swsRestraintTypeCylindricalFaces* swsRestraintType\_e.swsRestaintTypeReferenceGeometry* swsRestraintType\_e.swsRestraintTypeSphericalSurface
      - or -* swsRestraintType\_e.swsRestraintTypeFlatFace

| If the direction reference of this restraint is... | Then... |
| --- | --- |
| An axis or cylindrical face | * DVal1 is in the radial direction,* DVal2 is in the circumferential direction, and* DVal3 is in the axial direction. |
| A spherical face | * DVal1 is in the radial direction,* DVal2 is in the longitudinal direction, and* DVal3 is in the latitudinal direction. |
| A flat face | * DVal1 is about face direction 1,* DVal2 is about face direction 2, and* DVal3 is about the normal to the face. |
| A model edge | * DVal3 is about the edge. |

Call [ICWRestraint::SetReferenceGeometry](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~SetReferenceGeometry.html) to set the direction reference of this restraint.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html)

[ICWRestraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint_members.html)

[ICWRestraint::SetRotationComponentsValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~SetRotationComponentsValues.html)

[ICWRestraint::GetReverseDirections Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetReverseDirections.html)

[ICWRestraint::GetTranslationComponentsValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~GetTranslationComponentsValues.html)

[ICWRestraint::Unit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~Unit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0