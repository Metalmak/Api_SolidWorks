<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatPower~SetCutOffTemperatures.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetCutOffTemperatures Method (ICWHeatPower) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWHeatPower Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatPower.html) : SetCutOffTemperatures Method (ICWHeatPower) |

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

Sets the thermostat cut off temperatures (lower and upper bounds) used in heat power for transient thermal studies.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetCutOffTemperatures( _    ByVal DVal1 As System.Double, _    ByVal DVal2 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWHeatPower Dim DVal1 As System.Double Dim DVal2 As System.Double   instance.SetCutOffTemperatures(DVal1, DVal2) ``` | |

| C# |  |
| --- | --- |
| ``` void SetCutOffTemperatures(     System.double DVal1,    System.double DVal2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetCutOffTemperatures(  &   System.double DVal1, &   System.double DVal2 ) ``` | |

#### Parameters

*DVal1*
:   Lower-bound temperature

*DVal2*
:   Upper-bound temperature

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWHeatPower::SetCutOffTemperatures.

# ![](dotnetimages/collapse.gif)Example

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (C#)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_CSharp.htm)

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (VB.NET)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_VBNET.htm)

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (VBA)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWHeatPower Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatPower.html)

[ICWHeatPower Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatPower_members.html)

[ICWHeatPower::GetCutOffTemperatures Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWHeatPower~GetCutOffTemperatures.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0