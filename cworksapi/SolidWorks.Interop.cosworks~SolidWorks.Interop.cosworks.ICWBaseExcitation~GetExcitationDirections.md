<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetExcitationDirections Method (ICWBaseExcitation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html) : GetExcitationDirections Method (ICWBaseExcitation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BDir1*
:   1 to get excitation along plane direction 1, 0 to not (see **Remarks**)

*BDir2*
:   1 to get excitation along plane direction 2, 0 to not (see **Remarks**)

*BDir3*
:   1 to get excitation along plane direction 3, 0 to not (see **Remarks**)

Obsolete. Superseded by [ICWBaseExcitation::GetExcitationDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetExcitationDirections( _    ByRef BDir1 As System.Integer, _    ByRef BDir2 As System.Integer, _    ByRef BDir3 As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBaseExcitation Dim BDir1 As System.Integer Dim BDir2 As System.Integer Dim BDir3 As System.Integer   instance.GetExcitationDirections(BDir1, BDir2, BDir3) ``` | |

| C# |  |
| --- | --- |
| ``` void GetExcitationDirections(     out System.int BDir1,    out System.int BDir2,    out System.int BDir3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetExcitationDirections(  &   [Out] System.int BDir1, &   [Out] System.int BDir2, &   [Out] System.int BDir3 ) ``` | |

#### Parameters

*BDir1*
:   1 to get excitation along plane direction 1, 0 to not (see **Remarks**)

*BDir2*
:   1 to get excitation along plane direction 2, 0 to not (see **Remarks**)

*BDir3*
:   1 to get excitation along plane direction 3, 0 to not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWBaseExcitation::GetExcitationDirections.

# ![](dotnetimages/collapse.gif)Remarks

For uniform base excitations, this method is valid only if you did not call [ICWBaseExcitation::SetDirectionEntityForUniformExcitation](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~SetDirectionEntityForUniformExcitation.html) to set the face, edge, or plane in whose direction the excitation is uniformly applied.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html)

[ICWBaseExcitation Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation_members.html)

[ICWBaseExcitation::SetExcitationDirections Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetExcitationDirections.html)

[ICWBaseExcitation::GetExcitationDirectionValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationDirectionValues.html)

[ICWBaseExcitation::GetExcitationReverseDirections Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationReverseDirections.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0