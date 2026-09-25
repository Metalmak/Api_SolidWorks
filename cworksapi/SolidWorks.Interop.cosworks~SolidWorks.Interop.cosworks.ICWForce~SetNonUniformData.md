<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetNonUniformData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetNonUniformData Method (ICWForce) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html) : SetNonUniformData Method (ICWForce) |

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
:   Coefficient of the Y term

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
| ``` Sub SetNonUniformData( _    ByVal DConstVal As System.Double, _    ByVal DX As System.Double, _    ByVal DY As System.Double, _    ByVal DXY As System.Double, _    ByVal DX2 As System.Double, _    ByVal DY2 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWForce Dim DConstVal As System.Double Dim DX As System.Double Dim DY As System.Double Dim DXY As System.Double Dim DX2 As System.Double Dim DY2 As System.Double   instance.SetNonUniformData(DConstVal, DX, DY, DXY, DX2, DY2) ``` | |

| C# |  |
| --- | --- |
| ``` void SetNonUniformData(     System.double DConstVal,    System.double DX,    System.double DY,    System.double DXY,    System.double DX2,    System.double DY2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetNonUniformData(  &   System.double DConstVal, &   System.double DX, &   System.double DY, &   System.double DXY, &   System.double DX2, &   System.double DY2 ) ``` | |

#### Parameters

*DConstVal*
:   Constant

*DX*
:   Coefficient of the X term

*DY*
:   Coefficient of the Y term

*DXY*
:   Coefficient of the XY term

*DX2*
:   Coefficient of the X2 term

*DY2*
:   Coefficient of the Y2 term

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWForce::SetNonUniformData.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [ICWForce::IncludeNonUniformDistribution2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~IncludeNonUniformDistribution2.html) is set to -1 or true.

See the SOLIDWORKS Simulation user-interface help for details.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html)

[ICWForce Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce_members.html)

[ICWForce::GetNonUniformData Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetNonUniformData.html)

[ICWForce::SetCoordinateSystem Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetCoordinateSystem.html)

[ICWForce::Equation Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~Equation.html)

[ICWForce::EquationAngularUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~EquationAngularUnit.html)

[ICWForce::EquationCoordinateSystemType Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~EquationCoordinateSystemType.html)

[ICWForce::EquationLinearUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~EquationLinearUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0