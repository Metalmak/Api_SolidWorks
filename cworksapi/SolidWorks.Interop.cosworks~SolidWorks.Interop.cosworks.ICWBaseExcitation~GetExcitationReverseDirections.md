<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationReverseDirections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetExcitationReverseDirections Method (ICWBaseExcitation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html) : GetExcitationReverseDirections Method (ICWBaseExcitation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BDir1*
:   1 to reverse plane direction 1, 0 to not; valid only if BDir1 = 1 in [ICWBaseExcitation::GetExcitationDirections](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections.html) (see **Remarks**)

*BDir2*
:   1 to reverse plane direction 2, 0 to not; valid only if BDir2 = 1 in ICWBaseExcitation::GetExcitationDirections (see **Remarks**)

*BDir3*
:   1 to reverse plane direction 3, 0 to not; valid only if BDir3 = 1 in ICWBaseExcitation::GetExcitationDirections (see **Remarks**)

*BReversePhaseAngle*
:   1 to reverse phase angle, 0 to not

Obsolete. Superseded by [ICWBaseExcitation::GetExcitationReverseDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationReverseDirections2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetExcitationReverseDirections( _    ByRef BDir1 As System.Integer, _    ByRef BDir2 As System.Integer, _    ByRef BDir3 As System.Integer, _    ByRef BReversePhaseAngle As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBaseExcitation Dim BDir1 As System.Integer Dim BDir2 As System.Integer Dim BDir3 As System.Integer Dim BReversePhaseAngle As System.Integer   instance.GetExcitationReverseDirections(BDir1, BDir2, BDir3, BReversePhaseAngle) ``` | |

| C# |  |
| --- | --- |
| ``` void GetExcitationReverseDirections(     out System.int BDir1,    out System.int BDir2,    out System.int BDir3,    out System.int BReversePhaseAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetExcitationReverseDirections(  &   [Out] System.int BDir1, &   [Out] System.int BDir2, &   [Out] System.int BDir3, &   [Out] System.int BReversePhaseAngle ) ``` | |

#### Parameters

*BDir1*
:   1 to reverse plane direction 1, 0 to not; valid only if BDir1 = 1 in [ICWBaseExcitation::GetExcitationDirections](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections.html) (see **Remarks**)

*BDir2*
:   1 to reverse plane direction 2, 0 to not; valid only if BDir2 = 1 in ICWBaseExcitation::GetExcitationDirections (see **Remarks**)

*BDir3*
:   1 to reverse plane direction 3, 0 to not; valid only if BDir3 = 1 in ICWBaseExcitation::GetExcitationDirections (see **Remarks**)

*BReversePhaseAngle*
:   1 to reverse phase angle, 0 to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWBaseExcitation::GetExcitationReverseDirections.

# ![](dotnetimages/collapse.gif)Remarks

For uniform base excitations, this method is valid only if you did not call [ICWBaseExcitation::SetDirectionEntityForUniformExcitation](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~SetDirectionEntityForUniformExcitation.html) to set the face, edge, or plane in whose direction the excitation is uniformly applied.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html)

[ICWBaseExcitation Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation_members.html)

[ICWBaseExcitation::SetExcitationReverseDirections Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetExcitationReverseDirections.html)

[ICWBaseExcitation::GetExcitationDirectionValues Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationDirectionValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0