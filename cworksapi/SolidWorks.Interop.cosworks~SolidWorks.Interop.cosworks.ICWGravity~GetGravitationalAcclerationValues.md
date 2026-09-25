<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~GetGravitationalAcclerationValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetGravitationalAcclerationValues Method (ICWGravity) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWGravity Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity.html) : GetGravitationalAcclerationValues Method (ICWGravity) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DVal1*
:   Acceleration of gravity in plane direction 1

*DVal2*
:   Acceleration of gravity in plane direction 2

*DVal3*
:   Acceleration of gravity in the direction normal to the plane

Gets the gravitational acceleration values.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetGravitationalAcclerationValues( _    ByRef DVal1 As System.Double, _    ByRef DVal2 As System.Double, _    ByRef DVal3 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWGravity Dim DVal1 As System.Double Dim DVal2 As System.Double Dim DVal3 As System.Double   instance.GetGravitationalAcclerationValues(DVal1, DVal2, DVal3) ``` | |

| C# |  |
| --- | --- |
| ``` void GetGravitationalAcclerationValues(     out System.double DVal1,    out System.double DVal2,    out System.double DVal3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetGravitationalAcclerationValues(  &   [Out] System.double DVal1, &   [Out] System.double DVal2, &   [Out] System.double DVal3 ) ``` | |

#### Parameters

*DVal1*
:   Acceleration of gravity in plane direction 1

*DVal2*
:   Acceleration of gravity in plane direction 2

*DVal3*
:   Acceleration of gravity in the direction normal to the plane

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWGravity::GetGravitationalAcclerationValues.

# ![](dotnetimages/collapse.gif)Example

See the [ICWGravity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWGravity Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity.html)

[ICWGravity Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity_members.html)

[ICWGravity::SetGravitationalAcclerationValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~SetGravitationalAcclerationValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0