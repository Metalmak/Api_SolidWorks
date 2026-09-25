<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetExcitationDirections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetExcitationDirections Method (ICWBaseExcitation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html) : SetExcitationDirections Method (ICWBaseExcitation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BDir1*
:   1 to set excitation along plane direction 1, 0 to not (see **Remarks**)

*BDir2*
:   1 to set excitation along plane direction 2, 0 to not (see **Remarks**)

*BDir3*
:   1 to set excitation along plane direction 3, 0 to not (see **Remarks**)

Obsolete. Superseded by [ICWBaseExcitation::setExcitationDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetExcitationDirections2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetExcitationDirections( _    ByVal BDir1 As System.Integer, _    ByVal BDir2 As System.Integer, _    ByVal BDir3 As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBaseExcitation Dim BDir1 As System.Integer Dim BDir2 As System.Integer Dim BDir3 As System.Integer   instance.SetExcitationDirections(BDir1, BDir2, BDir3) ``` | |

| C# |  |
| --- | --- |
| ``` void SetExcitationDirections(     System.int BDir1,    System.int BDir2,    System.int BDir3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetExcitationDirections(  &   System.int BDir1, &   System.int BDir2, &   System.int BDir3 ) ``` | |

#### Parameters

*BDir1*
:   1 to set excitation along plane direction 1, 0 to not (see **Remarks**)

*BDir2*
:   1 to set excitation along plane direction 2, 0 to not (see **Remarks**)

*BDir3*
:   1 to set excitation along plane direction 3, 0 to not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWBaseExcitation::SetExcitationDirections.

# ![](dotnetimages/collapse.gif)Remarks

For uniform base excitations, you can specify the direction of excitation by calling either:

* this method, [ICWBaseExcitation::SetExcitationDirectionValues](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~SetExcitationDirectionValues.html), and [ICWBaseExcitation::SetExcitationReverseDirections](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetExcitationReverseDirections.html) to explicitly specify the excitation direction components and values

- or -

* [ICWBaseExcitation::SetDirectionEntityForUniformExcitation](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~SetDirectionEntityForUniformExcitation.html) to specify the face, edge, or plane in whose direction the excitation is uniformly applied.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html)

[ICWBaseExcitation Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation_members.html)

[ICWBaseExcitation::GetExcitationDirections Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0