<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetHeatPowerOrEnergy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetHeatPowerOrEnergy Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetHeatPowerOrEnergy Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BHeatEnergy*
:   0 for heat power, 1 for heat energy

*ArraySelectedEntities*
:   Array of geometric entities

*NUnits*
:   Units as defined in [swsUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnit_e.html)

*NStepNumber*
:   Solution step number (use 1 for steady state)

*NStepNumber2*
:   End solution step number (use 1 for steady state); valid only if BHeatEnergy is 1

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Obsolete. Superseded by [ICWResults::GetHeatPowerOrEnergy2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetHeatPowerOrEnergy2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetHeatPowerOrEnergy( _    ByVal BHeatEnergy As System.Integer, _    ByVal ArraySelectedEntities As System.Object, _    ByVal NUnits As System.Integer, _    ByVal NStepNumber As System.Integer, _    ByVal NStepNumber2 As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim BHeatEnergy As System.Integer Dim ArraySelectedEntities As System.Object Dim NUnits As System.Integer Dim NStepNumber As System.Integer Dim NStepNumber2 As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetHeatPowerOrEnergy(BHeatEnergy, ArraySelectedEntities, NUnits, NStepNumber, NStepNumber2, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetHeatPowerOrEnergy(     System.int BHeatEnergy,    System.object ArraySelectedEntities,    System.int NUnits,    System.int NStepNumber,    System.int NStepNumber2,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetHeatPowerOrEnergy(  &   System.int BHeatEnergy, &   System.Object^ ArraySelectedEntities, &   System.int NUnits, &   System.int NStepNumber, &   System.int NStepNumber2, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*BHeatEnergy*
:   0 for heat power, 1 for heat energy

*ArraySelectedEntities*
:   Array of geometric entities

*NUnits*
:   Units as defined in [swsUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnit_e.html)

*NStepNumber*
:   Solution step number (use 1 for steady state)

*NStepNumber2*
:   End solution step number (use 1 for steady state); valid only if BHeatEnergy is 1

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

#### Return Value

Array of heat values (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetHeatPowerOrEnergy.

# ![](dotnetimages/collapse.gif)Remarks

This method returns the following array:

{

*sel\_power\_or\_energy\_in*,

*sel\_power\_or\_energy\_out*,

*sel\_net\_power*,

*model\_power\_or\_energy\_in*,

*model\_power\_or\_energy\_out*,

*model\_net\_power\_or\_energy*

},

where *sel\_power\_or\_energy\_in* and *sel\_power\_or\_energy\_out* are the sum of individual entity in and out values, and *model\_power\_or\_energy\_in* and *model\_power\_or\_energy\_out* are total in and out values for the entire model.

*sel\_net\_power* = (*sel\_power\_or\_energy\_in* - *sel\_power\_or\_energy\_out)*

*model\_net\_power\_or\_energy* = (*model\_power\_or\_energy\_in* - *model\_power\_or\_energy\_out)*

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetMinMaxThermal Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxThermal.html)

[ICWResults::GetThermalComponentForAllStepsAtNode Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetThermalComponentForAllStepsAtNode.html)

[ICWResults::GetThermalForEntities Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetThermalForEntities.html)

[ICWResults::GetThermalValues Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetThermalValues.html)

[ICWResults::GetThermalValuesAtPoints Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetThermalValuesAtPoints.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0