<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~SetWeldSizingSettingEuro.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetWeldSizingSettingEuro Method (ICWEdgeWeldConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWEdgeWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html) : SetWeldSizingSettingEuro Method (ICWEdgeWeldConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NWeakMaterial*
:   Material of weaker joined part as defined in [swsWeakMaterial\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsWeakMaterial_e.html)

*DUltimateTensileStrength*
:   Ultimate tensile strength of NWeakMaterial

*NTensileStrengthUnit*
:   DUltimateTensileStrength units as defined in [swsWeldStrengthUnits\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsWeldStrengthUnits_e.html)

*DCorrelationFactor*
:   0.8 <= correlation factor for weld calculations <= 1.0

*DPartialSafetyFactor*
:   1.0 <= partial safety factor for joints <= 1.25

*BIsEstimatedWeldSize*
:   True to calculate the appropriate size for the weld connector and compare it to DEstimatedWeldSize in the Weld Check Plot; false to just use DEstimatedWeldSize

*DEstimatedWeldSize*
:   Estimated weld size

*NEstimatedWeldSizeUnit*
:   DEstimatedWeldSize units as defined in [swsEstimatedWeldSizeUnits\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEstimatedWeldSizeUnits_e.html)

Sets the European Standard settings for weld sizing calculations.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetWeldSizingSettingEuro( _    ByVal NWeakMaterial As System.Integer, _    ByVal DUltimateTensileStrength As System.Double, _    ByVal NTensileStrengthUnit As System.Integer, _    ByVal DCorrelationFactor As System.Double, _    ByVal DPartialSafetyFactor As System.Double, _    ByVal BIsEstimatedWeldSize As System.Boolean, _    ByVal DEstimatedWeldSize As System.Double, _    ByVal NEstimatedWeldSizeUnit As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWEdgeWeldConnector Dim NWeakMaterial As System.Integer Dim DUltimateTensileStrength As System.Double Dim NTensileStrengthUnit As System.Integer Dim DCorrelationFactor As System.Double Dim DPartialSafetyFactor As System.Double Dim BIsEstimatedWeldSize As System.Boolean Dim DEstimatedWeldSize As System.Double Dim NEstimatedWeldSizeUnit As System.Integer Dim value As System.Integer   value = instance.SetWeldSizingSettingEuro(NWeakMaterial, DUltimateTensileStrength, NTensileStrengthUnit, DCorrelationFactor, DPartialSafetyFactor, BIsEstimatedWeldSize, DEstimatedWeldSize, NEstimatedWeldSizeUnit) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetWeldSizingSettingEuro(     System.int NWeakMaterial,    System.double DUltimateTensileStrength,    System.int NTensileStrengthUnit,    System.double DCorrelationFactor,    System.double DPartialSafetyFactor,    System.bool BIsEstimatedWeldSize,    System.double DEstimatedWeldSize,    System.int NEstimatedWeldSizeUnit ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetWeldSizingSettingEuro(  &   System.int NWeakMaterial, &   System.double DUltimateTensileStrength, &   System.int NTensileStrengthUnit, &   System.double DCorrelationFactor, &   System.double DPartialSafetyFactor, &   System.bool BIsEstimatedWeldSize, &   System.double DEstimatedWeldSize, &   System.int NEstimatedWeldSizeUnit ) ``` | |

#### Parameters

*NWeakMaterial*
:   Material of weaker joined part as defined in [swsWeakMaterial\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsWeakMaterial_e.html)

*DUltimateTensileStrength*
:   Ultimate tensile strength of NWeakMaterial

*NTensileStrengthUnit*
:   DUltimateTensileStrength units as defined in [swsWeldStrengthUnits\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsWeldStrengthUnits_e.html)

*DCorrelationFactor*
:   0.8 <= correlation factor for weld calculations <= 1.0

*DPartialSafetyFactor*
:   1.0 <= partial safety factor for joints <= 1.25

*BIsEstimatedWeldSize*
:   True to calculate the appropriate size for the weld connector and compare it to DEstimatedWeldSize in the Weld Check Plot; false to just use DEstimatedWeldSize

*DEstimatedWeldSize*
:   Estimated weld size

*NEstimatedWeldSizeUnit*
:   DEstimatedWeldSize units as defined in [swsEstimatedWeldSizeUnits\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEstimatedWeldSizeUnits_e.html)

#### Return Value

Error code as defined in [swsWeldResultErrorCode\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsWeldResultErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWEdgeWeldConnector::SetWeldSizingSettingEuro.

# ![](dotnetimages/collapse.gif)Example

See the [ICWEdgeWeldConnector](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWEdgeWeldConnector::GetCodeType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWEdgeWeldConnector~GetCodeType.html) returns [swsEdgeWeldSolverCode\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEdgeWeldSolverCode_e.html).swsEdgeWeldSolverCodeEURO.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWEdgeWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html)

[ICWEdgeWeldConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector_members.html)

[ICWEdgeWeldConnector::GetWeldSizingSettingEuro Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~GetWeldSizingSettingEuro.html)

[ICWEdgeWeldConnector::SetWeldSizingSettingUS Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~SetWeldSizingSettingUS.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0