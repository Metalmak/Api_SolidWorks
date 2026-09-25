<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetExcitationDirections2 Method (ICWBaseExcitation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html) : GetExcitationDirections2 Method (ICWBaseExcitation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BDir1*
:   -1 or true to get excitation along plane direction 1, 0 or false to not (see **Remarks**)

*BDir2*
:   -1 or true to get excitation along plane direction 2, 0 or false to not (see **Remarks**)

*BDir3*
:   -1 or true to get excitation along plane direction 3, 0 or false to not (see **Remarks**)

Gets the directions in which this excitation is applied.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetExcitationDirections2( _    ByRef BDir1 As System.Boolean, _    ByRef BDir2 As System.Boolean, _    ByRef BDir3 As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBaseExcitation Dim BDir1 As System.Boolean Dim BDir2 As System.Boolean Dim BDir3 As System.Boolean   instance.GetExcitationDirections2(BDir1, BDir2, BDir3) ``` | |

| C# |  |
| --- | --- |
| ``` void GetExcitationDirections2(     out System.bool BDir1,    out System.bool BDir2,    out System.bool BDir3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetExcitationDirections2(  &   [Out] System.bool BDir1, &   [Out] System.bool BDir2, &   [Out] System.bool BDir3 ) ``` | |

#### Parameters

*BDir1*
:   -1 or true to get excitation along plane direction 1, 0 or false to not (see **Remarks**)

*BDir2*
:   -1 or true to get excitation along plane direction 2, 0 or false to not (see **Remarks**)

*BDir3*
:   -1 or true to get excitation along plane direction 3, 0 or false to not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [ICWBaseExcitation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

For uniform base excitations, this method is valid only if you did not call [ICWBaseExcitation::SetDirectionEntityForUniformExcitation](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~SetDirectionEntityForUniformExcitation.html) to set the face, edge, or plane in whose direction the excitation is uniformly applied.

This method returns booleans or integers in out parameters BDir1, BDir2, and BDir3, depending on their prior declarations.

If out parameters BDir1, BDir2, and BDir3 are cast as:

* Booleans, true or false is returned in each out parameter.* Longs or integers, -1 (=true) or 0 (=false) is returned in each out parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html)

[ICWBaseExcitation Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2022 SP0