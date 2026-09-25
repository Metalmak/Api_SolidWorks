<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetExcitationReverseDirections2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetExcitationReverseDirections2 Method (ICWBaseExcitation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html) : SetExcitationReverseDirections2 Method (ICWBaseExcitation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BDir1*
:   -1 or true to reverse plane direction 1, 0 or false to not (see **Remarks**)

*BDir2*
:   -1 or true to reverse plane direction 2, 0 or false to not (see **Remarks**)

*BDir3*
:   -1 or true to reverse plane direction 3, 0 or false to not (see **Remarks**)

*BReversePhaseAngle*
:   -1 or true to reverse phase angle, 0 or false to not (see **Remarks**)

Sets whether to reverse base excitation directions.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetExcitationReverseDirections2( _    ByVal BDir1 As System.Boolean, _    ByVal BDir2 As System.Boolean, _    ByVal BDir3 As System.Boolean, _    ByVal BReversePhaseAngle As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBaseExcitation Dim BDir1 As System.Boolean Dim BDir2 As System.Boolean Dim BDir3 As System.Boolean Dim BReversePhaseAngle As System.Boolean   instance.SetExcitationReverseDirections2(BDir1, BDir2, BDir3, BReversePhaseAngle) ``` | |

| C# |  |
| --- | --- |
| ``` void SetExcitationReverseDirections2(     System.bool BDir1,    System.bool BDir2,    System.bool BDir3,    System.bool BReversePhaseAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetExcitationReverseDirections2(  &   System.bool BDir1, &   System.bool BDir2, &   System.bool BDir3, &   System.bool BReversePhaseAngle ) ``` | |

#### Parameters

*BDir1*
:   -1 or true to reverse plane direction 1, 0 or false to not (see **Remarks**)

*BDir2*
:   -1 or true to reverse plane direction 2, 0 or false to not (see **Remarks**)

*BDir3*
:   -1 or true to reverse plane direction 3, 0 or false to not (see **Remarks**)

*BReversePhaseAngle*
:   -1 or true to reverse phase angle, 0 or false to not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

For uniform base excitations, you can specify the direction of excitation by calling:

* this method, [ICWBaseExcitation::SetExcitationDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetExcitationDirections2.html), and [ICWBaseExcitation::SetExcitationDirectionValues](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetExcitationDirectionValues.html) to explicitly specify the excitation direction components and values

    - or -

* [ICWBaseExcitation::SetDirectionEntityForUniformExcitation](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~SetDirectionEntityForUniformExcitation.html) to specify the face, edge, or plane in whose direction the excitation is uniformly applied.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html)

[ICWBaseExcitation Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2022 SP0