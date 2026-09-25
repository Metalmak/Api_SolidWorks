<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~GetNonUniformData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetNonUniformData Method (ICWPressure) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPressure Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure.html) : GetNonUniformData Method (ICWPressure) |

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

*DXX*
:   Coefficient of the X2 term

*DYY*
:   Coefficient of the Y2 term

Obsolete. Superseded by [ICWPressure::Equation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~Equation.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetNonUniformData( _    ByRef DConstVal As System.Double, _    ByRef DX As System.Double, _    ByRef DY As System.Double, _    ByRef DXY As System.Double, _    ByRef DXX As System.Double, _    ByRef DYY As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPressure Dim DConstVal As System.Double Dim DX As System.Double Dim DY As System.Double Dim DXY As System.Double Dim DXX As System.Double Dim DYY As System.Double   instance.GetNonUniformData(DConstVal, DX, DY, DXY, DXX, DYY) ``` | |

| C# |  |
| --- | --- |
| ``` void GetNonUniformData(     out System.double DConstVal,    out System.double DX,    out System.double DY,    out System.double DXY,    out System.double DXX,    out System.double DYY ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetNonUniformData(  &   [Out] System.double DConstVal, &   [Out] System.double DX, &   [Out] System.double DY, &   [Out] System.double DXY, &   [Out] System.double DXX, &   [Out] System.double DYY ) ``` | |

#### Parameters

*DConstVal*
:   Constant

*DX*
:   Coefficient of the X term

*DY*
:   Coefficient of the Y term

*DXY*
:   Coefficient of the XY term

*DXX*
:   Coefficient of the X2 term

*DYY*
:   Coefficient of the Y2 term

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPressure::GetNonUniformData.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWPressure::IncludeNonUniformDistribution](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~IncludeNonUniformDistribution.html) is set to true.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPressure Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure.html)

[ICWPressure Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure_members.html)

[ICWPressure::SetNonUniformData Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~SetNonUniformData.html)

[ICWPressure::IncludeNonUniformDistribution Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~IncludeNonUniformDistribution.html)

[ICWPressure::EquationAngularUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~EquationAngularUnit.html)

[ICWPressure::EquationLinearUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~EquationLinearUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0