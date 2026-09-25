<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux~GetCutOffTemperatures.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetCutOffTemperatures Method (ICWHeatFlux) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWHeatFlux Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux.html) : GetCutOffTemperatures Method (ICWHeatFlux) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DVal1*
:   Lower-bound temperature

*DVal2*
:   Upper-bound temperature

Gets the thermostat lower- and upper-bound temperatures in this heat flux load.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetCutOffTemperatures( _    ByRef DVal1 As System.Double, _    ByRef DVal2 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWHeatFlux Dim DVal1 As System.Double Dim DVal2 As System.Double   instance.GetCutOffTemperatures(DVal1, DVal2) ``` | |

| C# |  |
| --- | --- |
| ``` void GetCutOffTemperatures(     out System.double DVal1,    out System.double DVal2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetCutOffTemperatures(  &   [Out] System.double DVal1, &   [Out] System.double DVal2 ) ``` | |

#### Parameters

*DVal1*
:   Lower-bound temperature

*DVal2*
:   Upper-bound temperature

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWHeatFlux::GetCutOffTemperatures.

# ![](dotnetimages/collapse.gif)Example

See the [ICWHeatFlux](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWHeatFlux Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux.html)

[ICWHeatFlux Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux_members.html)

[ICWHeatFlux::SetCutOffTemperatures Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatFlux~SetCutOffTemperatures.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0