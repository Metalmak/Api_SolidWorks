<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~SetRayleighDampingCoefficients.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetRayleighDampingCoefficients Method (ICWDampingOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDampingOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions.html) : SetRayleighDampingCoefficients Method (ICWDampingOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DAlpha*
:   Mass coefficient

*DBeta*
:   Stiffness coefficient

Sets the Rayleigh damping coefficients.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetRayleighDampingCoefficients( _    ByVal DAlpha As System.Double, _    ByVal DBeta As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDampingOptions Dim DAlpha As System.Double Dim DBeta As System.Double   instance.SetRayleighDampingCoefficients(DAlpha, DBeta) ``` | |

| C# |  |
| --- | --- |
| ``` void SetRayleighDampingCoefficients(     System.double DAlpha,    System.double DBeta ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetRayleighDampingCoefficients(  &   System.double DAlpha, &   System.double DBeta ) ``` | |

#### Parameters

*DAlpha*
:   Mass coefficient

*DBeta*
:   Stiffness coefficient

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDampingOptions::SetRayleighDampingCoefficients.

# ![](dotnetimages/collapse.gif)Remarks

This method works only if [ICWDampingOptions::DampingType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDampingOptions~DampingType.html) is set to [swsDampingType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDampingType_e.html).swsDampingType\_Rayleigh.

For more information about Rayleigh damping, see the SOLIDWORKS Simulation Help.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDampingOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions.html)

[ICWDampingOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions_members.html)

[ICWDampingOptions::GetRayleighDampingCoefficients Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~GetRayleighDampingCoefficients.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0