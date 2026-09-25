<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~GetZeroStrainTemperature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetZeroStrainTemperature Method (ICWNonLinearStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) : GetZeroStrainTemperature Method (ICWNonLinearStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DZeroStrainTemperature*
:   Reference temperature at zero strain

*NZeroStrainTemperatureUnit*
:   Temperature units as defined [swsTemperatureUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsTemperatureUnit_e.html)

Gets the temperature at zero strain and its units.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetZeroStrainTemperature( _    ByRef DZeroStrainTemperature As System.Double, _    ByRef NZeroStrainTemperatureUnit As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWNonLinearStudyOptions Dim DZeroStrainTemperature As System.Double Dim NZeroStrainTemperatureUnit As System.Integer   instance.GetZeroStrainTemperature(DZeroStrainTemperature, NZeroStrainTemperatureUnit) ``` | |

| C# |  |
| --- | --- |
| ``` void GetZeroStrainTemperature(     out System.double DZeroStrainTemperature,    out System.int NZeroStrainTemperatureUnit ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetZeroStrainTemperature(  &   [Out] System.double DZeroStrainTemperature, &   [Out] System.int NZeroStrainTemperatureUnit ) ``` | |

#### Parameters

*DZeroStrainTemperature*
:   Reference temperature at zero strain

*NZeroStrainTemperatureUnit*
:   Temperature units as defined [swsTemperatureUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsTemperatureUnit_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWNonLinearStudyOptions::GetZeroStrainTemperature.

# ![](dotnetimages/collapse.gif)Remarks

The default temperature at zero strain is 298 Kelvin.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWNonLinearStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html)

[ICWNonLinearStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions_members.html)

[ICWNonLinearStudyOptions::SetZeroStrainTemperature Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~SetZeroStrainTemperature.html)

[ICWNonLinearStudyOptions::UseLargeStrain Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions~UseLargeStrain.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0