<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreatePlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CreatePlot Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : CreatePlot Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NResultType*
:   Type of results plot as defined by [swsPlotResultTypes\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotResultTypes_e.html) (see **Remarks**)

*NComponent*
:   Component to plot (see **Remarks**)

*NUnits*
:   Units as appropriate to NComponent (see **Remarks**)

*BValueByElem*
:   True to plot element values, false to plot node values

*ErrorCode*
:   Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

Creates the specified plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreatePlot( _    ByVal NResultType As System.Integer, _    ByVal NComponent As System.Integer, _    ByVal NUnits As System.Integer, _    ByVal BValueByElem As System.Boolean, _    ByRef ErrorCode As System.Integer _ ) As CWPlot ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim NResultType As System.Integer Dim NComponent As System.Integer Dim NUnits As System.Integer Dim BValueByElem As System.Boolean Dim ErrorCode As System.Integer Dim value As CWPlot   value = instance.CreatePlot(NResultType, NComponent, NUnits, BValueByElem, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWPlot CreatePlot(     System.int NResultType,    System.int NComponent,    System.int NUnits,    System.bool BValueByElem,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWPlot^ CreatePlot(  &   System.int NResultType, &   System.int NComponent, &   System.int NUnits, &   System.bool BValueByElem, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NResultType*
:   Type of results plot as defined by [swsPlotResultTypes\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotResultTypes_e.html) (see **Remarks**)

*NComponent*
:   Component to plot (see **Remarks**)

*NUnits*
:   Units as appropriate to NComponent (see **Remarks**)

*BValueByElem*
:   True to plot element values, false to plot node values

*ErrorCode*
:   Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

#### Return Value

[ICWPlot](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::CreatePlot.

# ![](dotnetimages/collapse.gif)Example

[Create Plots for Static Study (VBA)](Create_Plots_for_Static_Study_Example_VB.htm)

[Create Plots for Static Study (VB.NET)](Create_Plots_for_Static_Study_Example_VBNET.htm)

[Create Plots for Static Study (C#)](Create_Plots_for_Static_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

| If NResultType is swsPlotResultTypes\_e... | Then NComponent contains the component to plot as defined by... | And NUnits contains the units as defined by... |
| --- | --- | --- |
| swsResultAcceleration | [swsAccelerationComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsAccelerationComponent_e.html) | [swsAccelerationUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsAccelerationUnit_e.html) |
| swsResultBeamDiagram | [swsBeamForceType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsBeamForceType_e.html) | [swsForceUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsForceUnit_e.html) |
| swsResultBeamStress | [swsBeamStressType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsBeamStressType_e.html) | [swsStrengthUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStrengthUnit_e.html) |
| swsResultDesignInsight | N/A | N/A |
| swsResultDisplacementOrAmplitude | * [swsDisplacementComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsDisplacementComponent_e.html) (Displacement)* [swsFrequencyBucklingResultDisplacementComponentTypes\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFrequencyBucklingResultDisplacementComponentTypes_e.html) (Amplitude for frequency and buckling studies) | [swsLinearUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinearUnit_e.html) (displacement) or [swsForceUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsForceUnit_e.html) (reaction force) |
| swsResultEdgeWeldConnector | N/A | N/A |
| swsResultFactorOfSafety | * [swsFOS\_NonCompositeCriterion\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_NonCompositeCriterion_e.html) (Non-composite shells)* [swsFOS\_CompositeCriterion\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_CompositeCriterion_e.html) (Composite shells) | N/A |
| swsResultFatigue | [swsFatigueComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFatigueComponent_e.html) | N/A |
| swsResultPinBoltBearing | N/A | N/A |
| swsResultStrain | [swsStrainComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStrainComponent_e.html) | [swsStrengthUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStrengthUnit_e.html) |
| swsResultEquivalentStress\* | N/A | [swsStrengthUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStrengthUnit_e.html) |
| swsResultStress | [swsStressComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStressComponent_e.html) | [swsStrengthUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStrengthUnit_e.html) |
| swsResultThermal | [swsThermalComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsThermalComponent_e.html) | [swsTemperatureUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTemperatureUnit_e.html) |
| swsResultVelocity | [swsVelocityComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsVelocityComponent_e.html) | [swsVelocityUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsVelocityUnit_e.html) |

\*The following conditions are required to create an equivalent stress plot:

* Mixed mesh model with beams and solids/shells* Dynamic study* **Nodal von Mises stress only (Faster)** option is chosen in **Results Options > Quantity** to calculate stress results

**NOTE:** After calling this method to create a plot of linear dynamic, frequency, or buckling studies, call [ICWPlot::SetModeShape](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~SetModeShape.html) to set the mode shape number of the plot.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::ActivatePlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~ActivatePlot.html)

[ICWResults::DeletePlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~DeletePlot.html)

[ICWResults::GetPlotColorOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotColorOptions.html)

[ICWResults::GetPlotCount Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotCount.html)

[ICWResults::GetPlotDisplayOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotDisplayOptions.html)

[ICWResults::GetPlotPositionFormatOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotPositionFormatOptions.html)

[ICWResults::GetPlotSettings Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotSettings.html)

[ICWResults::SavePlotsAseDrawings Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SavePlotsAseDrawings.html)

[ICWResults::SetPlotColorOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotColorOptions.html)

[ICWResults::SetPlotDisplayOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotDisplayOptions.html)

[ICWResults::SetPlotPositionFormatOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotPositionFormatOptions.html)

[ICWResults::SetPlotSettings Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotSettings.html)

[ICWResults::AddIsoClippingToPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~AddIsoClippingToPlot.html)

[ICWResults::GetPlotNames Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotNames.html)

[ICWResults::GetPlotSettingsOptionForHiddenAndExcludedBody Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotSettingsOptionForHiddenAndExcludedBody.html)

[ICWResults::SetPlotSettingsOptionForHiddenAndExcludedBody Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetPlotSettingsOptionForHiddenAndExcludedBody.html)

[ICWResults::CreateResultsEquationPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateResultsEquationPlot.html)

[ICWPlot::SetComponentUnitAndValueByElem Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~SetComponentUnitAndValueByElem.html)

[ICWResults::GetPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlot.html)

[ICWResults::CreateStressHotSpotPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateStressHotSpotPlot.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0