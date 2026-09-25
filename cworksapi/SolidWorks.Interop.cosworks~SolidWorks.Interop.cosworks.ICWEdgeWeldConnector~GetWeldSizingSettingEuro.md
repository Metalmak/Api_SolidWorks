<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~GetWeldSizingSettingEuro.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetWeldSizingSettingEuro Method (ICWEdgeWeldConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWEdgeWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html) : GetWeldSizingSettingEuro Method (ICWEdgeWeldConnector) |

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

Gets the European Standard settings for weld sizing calculations.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetWeldSizingSettingEuro( _    ByRef NWeakMaterial As System.Integer, _    ByRef DUltimateTensileStrength As System.Double, _    ByRef NTensileStrengthUnit As System.Integer, _    ByRef DCorrelationFactor As System.Double, _    ByRef DPartialSafetyFactor As System.Double, _    ByRef BIsEstimatedWeldSize As System.Boolean, _    ByRef DEstimatedWeldSize As System.Double, _    ByRef NEstimatedWeldSizeUnit As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWEdgeWeldConnector Dim NWeakMaterial As System.Integer Dim DUltimateTensileStrength As System.Double Dim NTensileStrengthUnit As System.Integer Dim DCorrelationFactor As System.Double Dim DPartialSafetyFactor As System.Double Dim BIsEstimatedWeldSize As System.Boolean Dim DEstimatedWeldSize As System.Double Dim NEstimatedWeldSizeUnit As System.Integer Dim value As System.Integer   value = instance.GetWeldSizingSettingEuro(NWeakMaterial, DUltimateTensileStrength, NTensileStrengthUnit, DCorrelationFactor, DPartialSafetyFactor, BIsEstimatedWeldSize, DEstimatedWeldSize, NEstimatedWeldSizeUnit) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetWeldSizingSettingEuro(     out System.int NWeakMaterial,    out System.double DUltimateTensileStrength,    out System.int NTensileStrengthUnit,    out System.double DCorrelationFactor,    out System.double DPartialSafetyFactor,    out System.bool BIsEstimatedWeldSize,    out System.double DEstimatedWeldSize,    out System.int NEstimatedWeldSizeUnit ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetWeldSizingSettingEuro(  &   [Out] System.int NWeakMaterial, &   [Out] System.double DUltimateTensileStrength, &   [Out] System.int NTensileStrengthUnit, &   [Out] System.double DCorrelationFactor, &   [Out] System.double DPartialSafetyFactor, &   [Out] System.bool BIsEstimatedWeldSize, &   [Out] System.double DEstimatedWeldSize, &   [Out] System.int NEstimatedWeldSizeUnit ) ``` | |

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

See CWEdgeWeldConnector::GetWeldSizingSettingEuro.

# ![](dotnetimages/collapse.gif)Example

See the [ICWEdgeWeldConnector](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWEdgeWeldConnector::GetCodeType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWEdgeWeldConnector~GetCodeType.html) returns [swsEdgeWeldSolverCode\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEdgeWeldSolverCode_e.html).swsEdgeWeldSolverCodeEURO.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWEdgeWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html)

[ICWEdgeWeldConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector_members.html)

[ICWEdgeWeldConnector::SetWeldSizingSettingEuro Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~SetWeldSizingSettingEuro.html)

[ICWEdgeWeldConnector::GetWeldSizingSettingUS Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~GetWeldSizingSettingUS.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0