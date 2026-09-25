<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~SetComponentUnitAndValueByElem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetComponentUnitAndValueByElem Method (ICWPlot) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) : SetComponentUnitAndValueByElem Method (ICWPlot) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NComponent*
:   Component to plot (see **Remarks**)

*NUnits*
:   Units as appropriate for NComponent (see **Remarks**)

*BValueByElem*
:   True to plot element values, false to plot node values

Sets the component, units, and values to plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetComponentUnitAndValueByElem( _    ByVal NComponent As System.Integer, _    ByVal NUnits As System.Integer, _    ByVal BValueByElem As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPlot Dim NComponent As System.Integer Dim NUnits As System.Integer Dim BValueByElem As System.Boolean Dim value As System.Integer   value = instance.SetComponentUnitAndValueByElem(NComponent, NUnits, BValueByElem) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetComponentUnitAndValueByElem(     System.int NComponent,    System.int NUnits,    System.bool BValueByElem ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetComponentUnitAndValueByElem(  &   System.int NComponent, &   System.int NUnits, &   System.bool BValueByElem ) ``` | |

#### Parameters

*NComponent*
:   Component to plot (see **Remarks**)

*NUnits*
:   Units as appropriate for NComponent (see **Remarks**)

*BValueByElem*
:   True to plot element values, false to plot node values

#### Return Value

Error code as defined by [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPlot::SetComponentUnitAndValueByElem.

# ![](dotnetimages/collapse.gif)Example

See the [ICWPlot](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

| If this plot's result type is swsPlotResultTypes\_e... | Then NComponent contains the component to plot as defined by... | And NUnits contains the units as defined by... |
| --- | --- | --- |
| swsResultAcceleration | [swsAccelerationComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsAccelerationComponent_e.html) | [swsAccelerationUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsAccelerationUnit_e.html) |
| swsResultBeamDiagram | [swsBeamForceType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsBeamForceType_e.html) | [swsForceUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsForceUnit_e.html) |
| swsResultBeamStress | [swsBeamStressType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsBeamStressType_e.html) | [swsStrengthUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStrengthUnit_e.html) |
| swsResultDesignInsight | N/A | N/A |
| swsResultDisplacementOrAmplitude | * [swsDisplacementComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsDisplacementComponent_e.html) (Displacement)* [swsFrequencyBucklingResultDisplacementComponentTypes\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFrequencyBucklingResultDisplacementComponentTypes_e.html) (Amplitude for frequency and buckling) | [swsLinearUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinearUnit_e.html) (displacement) or [swsForceUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsForceUnit_e.html) (reaction force) |
| swsResultEdgeWeldConnector | N/A | N/A |
| swsResultFactorOfSafety | * [swsFOS\_NonCompositeCriterion\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_NonCompositeCriterion_e.html) (Non-composite shells)* [swsFOS\_CompositeCriterion\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_CompositeCriterion_e.html) (Composite shells) | N/A |
| swsResultFatigue | [swsFatigueComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFatigueComponent_e.html) | N/A |
| swsResultPinBoltBearing | N/A | N/A |
| swsResultStrain | [swsStrainComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStrainComponent_e.html) | [swsStrengthUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStrengthUnit_e.html) |
| swsResultStress | [swsStressComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStressComponent_e.html) | [swsStrengthUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStrengthUnit_e.html) |
| swsResultThermal | [swsThermalComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsThermalComponent_e.html) | [swsTemperatureUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTemperatureUnit_e.html) |
| swsResultVelocity | [swsVelocityComponent\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsVelocityComponent_e.html) | [swsVelocityUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsVelocityUnit_e.html) |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html)

[ICWPlot Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot_members.html)

[ICWResults::CreatePlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreatePlot.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0