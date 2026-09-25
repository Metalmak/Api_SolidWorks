<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationReverseDirections2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetExcitationReverseDirections2 Method (ICWBaseExcitation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html) : GetExcitationReverseDirections2 Method (ICWBaseExcitation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BDir1*
:   -1 or true to reverse plane direction 1, 0 or false to not; valid only if BDir1 = -1 in [ICWBaseExcitation::GetExcitationDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections2.html) (see **Remarks**)

*BDir2*
:   -1 or true to reverse plane direction 2, 0 or false to not; valid only if BDir2 = -1 in ICWBaseExcitation::GetExcitationDirections2 (see **Remarks**)

*BDir3*
:   -1 or true to reverse plane direction 3, 0 or false to not; valid only if BDir3 = -1 in ICWBaseExcitation::GetExcitationDirections2 (see **Remarks**)

*BReversePhaseAngle*
:   -1 or true to reverse phase angle, 0 or false to not

Gets whether to reverse base excitation directions.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetExcitationReverseDirections2( _    ByRef BDir1 As System.Boolean, _    ByRef BDir2 As System.Boolean, _    ByRef BDir3 As System.Boolean, _    ByRef BReversePhaseAngle As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBaseExcitation Dim BDir1 As System.Boolean Dim BDir2 As System.Boolean Dim BDir3 As System.Boolean Dim BReversePhaseAngle As System.Boolean   instance.GetExcitationReverseDirections2(BDir1, BDir2, BDir3, BReversePhaseAngle) ``` | |

| C# |  |
| --- | --- |
| ``` void GetExcitationReverseDirections2(     out System.bool BDir1,    out System.bool BDir2,    out System.bool BDir3,    out System.bool BReversePhaseAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetExcitationReverseDirections2(  &   [Out] System.bool BDir1, &   [Out] System.bool BDir2, &   [Out] System.bool BDir3, &   [Out] System.bool BReversePhaseAngle ) ``` | |

#### Parameters

*BDir1*
:   -1 or true to reverse plane direction 1, 0 or false to not; valid only if BDir1 = -1 in [ICWBaseExcitation::GetExcitationDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections2.html) (see **Remarks**)

*BDir2*
:   -1 or true to reverse plane direction 2, 0 or false to not; valid only if BDir2 = -1 in ICWBaseExcitation::GetExcitationDirections2 (see **Remarks**)

*BDir3*
:   -1 or true to reverse plane direction 3, 0 or false to not; valid only if BDir3 = -1 in ICWBaseExcitation::GetExcitationDirections2 (see **Remarks**)

*BReversePhaseAngle*
:   -1 or true to reverse phase angle, 0 or false to not

# ![](dotnetimages/collapse.gif)Example

See the [ICWBaseExcitation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

For uniform base excitations, this method is valid only if you did not call [ICWBaseExcitation::SetDirectionEntityForUniformExcitation](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~SetDirectionEntityForUniformExcitation.html) to set the face, edge, or plane in whose direction the excitation is uniformly applied.

This method returns booleans or integers in out parameters BDir1, BDir2, BDir3, and BReversePhaseAngle, depending on their prior declarations.

If out parameters BDir1, BDir2, BDir3, BReversePhaseAngle are cast as:

* Booleans, true or false is returned in each out parameter.* Longs or integers, -1 (=true) or 0 (=false) is returned in each out parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html)

[ICWBaseExcitation Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2022 SP0