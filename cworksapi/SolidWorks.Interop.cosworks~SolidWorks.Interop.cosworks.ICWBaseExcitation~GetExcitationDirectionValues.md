<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationDirectionValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetExcitationDirectionValues Method (ICWBaseExcitation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html) : GetExcitationDirectionValues Method (ICWBaseExcitation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DVal1*
:   Excitation along plane direction 1; valid only if BDir1 = 1 in [ICWBaseExcitation::GetExcitationDirections](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections.html) (see **Remarks**)

*DVal2*
:   Excitation along plane direction 2; valid only if BDir2 = 1 in [ICWBaseExcitation::GetExcitationDirections](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections.html) (see **Remarks**)

*DVal3*
:   Excitation along plane direction 3; valid only if BDir3 = 1 in [ICWBaseExcitation::GetExcitationDirections](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections.html) (see **Remarks**)

Gets the excitation values in each direction.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetExcitationDirectionValues( _    ByRef DVal1 As System.Double, _    ByRef DVal2 As System.Double, _    ByRef DVal3 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBaseExcitation Dim DVal1 As System.Double Dim DVal2 As System.Double Dim DVal3 As System.Double   instance.GetExcitationDirectionValues(DVal1, DVal2, DVal3) ``` | |

| C# |  |
| --- | --- |
| ``` void GetExcitationDirectionValues(     out System.double DVal1,    out System.double DVal2,    out System.double DVal3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetExcitationDirectionValues(  &   [Out] System.double DVal1, &   [Out] System.double DVal2, &   [Out] System.double DVal3 ) ``` | |

#### Parameters

*DVal1*
:   Excitation along plane direction 1; valid only if BDir1 = 1 in [ICWBaseExcitation::GetExcitationDirections](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections.html) (see **Remarks**)

*DVal2*
:   Excitation along plane direction 2; valid only if BDir2 = 1 in [ICWBaseExcitation::GetExcitationDirections](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections.html) (see **Remarks**)

*DVal3*
:   Excitation along plane direction 3; valid only if BDir3 = 1 in [ICWBaseExcitation::GetExcitationDirections](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~GetExcitationDirections.html) (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWBaseExcitation::GetExcitationDirectionValues.

# ![](dotnetimages/collapse.gif)Example

[Create Linear Dynamic Study (VBA)](Create_Dynamic_Harmonic_Study_Example_VB.htm)

[Create Linear Dynamic Study (VB.NET)](Create_Dynamic_Harmonic_Study_Example_VBNET.htm)

[Create Linear Dynamic Study (C#)](Create_Dynamic_Harmonic_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

For uniform base excitations, this method is valid only if you did not call [ICWBaseExcitation::SetDirectionEntityForUniformExcitation](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation~SetDirectionEntityForUniformExcitation.html) to set the face, edge, or plane in whose direction the excitation is uniformly applied.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBaseExcitation Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation.html)

[ICWBaseExcitation Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation_members.html)

[ICWBaseExcitation::SetExcitationDirectionValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~SetExcitationDirectionValues.html)

[ICWBaseExcitation::Unit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~Unit.html)

[ICWBaseExcitation::GetExcitationReverseDirections Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBaseExcitation~GetExcitationReverseDirections.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0