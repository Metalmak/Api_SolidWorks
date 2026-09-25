<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetNonUniformData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetNonUniformData Method (ICWForce) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html) : GetNonUniformData Method (ICWForce) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DConstVal*
:   Constant

*DX*
:   Coefficient of the X term

*DY*
:   Coefficient of the Y term

*DXY*
:   Coefficient of the XY term

*DX2*
:   Coefficient of the X2 term

*DY2*
:   Coefficient of the Y2 term

Obsolete. Superseded by [ICWForce::Equation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~Equation.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetNonUniformData( _    ByRef DConstVal As System.Double, _    ByRef DX As System.Double, _    ByRef DY As System.Double, _    ByRef DXY As System.Double, _    ByRef DX2 As System.Double, _    ByRef DY2 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWForce Dim DConstVal As System.Double Dim DX As System.Double Dim DY As System.Double Dim DXY As System.Double Dim DX2 As System.Double Dim DY2 As System.Double   instance.GetNonUniformData(DConstVal, DX, DY, DXY, DX2, DY2) ``` | |

| C# |  |
| --- | --- |
| ``` void GetNonUniformData(     out System.double DConstVal,    out System.double DX,    out System.double DY,    out System.double DXY,    out System.double DX2,    out System.double DY2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetNonUniformData(  &   [Out] System.double DConstVal, &   [Out] System.double DX, &   [Out] System.double DY, &   [Out] System.double DXY, &   [Out] System.double DX2, &   [Out] System.double DY2 ) ``` | |

#### Parameters

*DConstVal*
:   Constant

*DX*
:   Coefficient of the X term

*DY*
:   Coefficient of the Y term

*DXY*
:   Coefficient of the XY term

*DX2*
:   Coefficient of the X2 term

*DY2*
:   Coefficient of the Y2 term

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWForce::GetNonUniformData.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [ICWForce::IncludeNonUniformDistribution2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~IncludeNonUniformDistribution2.html) is set to -1 or true.

See the SOLIDWORKS Simulation user-interface help for details about nonuniform force distribution.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html)

[ICWForce Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce_members.html)

[ICWForce::SetNonUniformData Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetNonUniformData.html)

[ICWForce::GetCoordinateSystem Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetCoordinateSystem.html)

[ICWForce::Equation Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~Equation.html)

[ICWForce::EquationAngularUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~EquationAngularUnit.html)

[ICWForce::EquationCoordinateSystemType Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~EquationCoordinateSystemType.html)

[ICWForce::EquationLinearUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~EquationLinearUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0