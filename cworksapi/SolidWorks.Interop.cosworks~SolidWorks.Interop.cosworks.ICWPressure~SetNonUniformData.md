<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~SetNonUniformData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetNonUniformData Method (ICWPressure) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPressure Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure.html) : SetNonUniformData Method (ICWPressure) |

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
| ``` Sub SetNonUniformData( _    ByVal DConstVal As System.Double, _    ByVal DX As System.Double, _    ByVal DY As System.Double, _    ByVal DXY As System.Double, _    ByVal DXX As System.Double, _    ByVal DYY As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPressure Dim DConstVal As System.Double Dim DX As System.Double Dim DY As System.Double Dim DXY As System.Double Dim DXX As System.Double Dim DYY As System.Double   instance.SetNonUniformData(DConstVal, DX, DY, DXY, DXX, DYY) ``` | |

| C# |  |
| --- | --- |
| ``` void SetNonUniformData(     System.double DConstVal,    System.double DX,    System.double DY,    System.double DXY,    System.double DXX,    System.double DYY ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetNonUniformData(  &   System.double DConstVal, &   System.double DX, &   System.double DY, &   System.double DXY, &   System.double DXX, &   System.double DYY ) ``` | |

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

See CWPressure::SetNonUniformData.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWPressure::IncludeNonUniformDistribution](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~IncludeNonUniformDistribution.html) is set to true.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPressure Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure.html)

[ICWPressure Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure_members.html)

[ICWPressure::GetNonUniformData Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~GetNonUniformData.html)

[ICWPressure::IncludeNonUniformDistribution Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~IncludeNonUniformDistribution.html)

[ICWPressure::EquationAngularUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~EquationAngularUnit.html)

[ICWPressure::EquationLinearUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~EquationLinearUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0