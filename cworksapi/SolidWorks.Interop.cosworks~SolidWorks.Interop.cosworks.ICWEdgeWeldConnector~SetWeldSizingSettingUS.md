<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~SetWeldSizingSettingUS.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetWeldSizingSettingUS Method (ICWEdgeWeldConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWEdgeWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html) : SetWeldSizingSettingUS Method (ICWEdgeWeldConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NElectrodeMaterial*
:   Electrode material as defined in [swsElectrodeMaterialTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsElectrodeMaterialTypes_e.html)

*DWeldStrength*
:   Ultimate shear strength of NElectrodeMaterial; if NElectrodeMaterial is swsElectrodeMaterialTypes\_e.swsElectrodeMaterialCustomAl or swsElectrodeMaterialTypes\_e.swsElectrodeMaterialCustomSteel, ultimate shear strength for the weld throat

*NWeldStrengthUnit*
:   DWeldStrength units as defined in [swsWeldStrengthUnits\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsWeldStrengthUnits_e.html)

*NSafetyFactorLiftOption*
:   Lift safety factor by which to reduce DWeldStrength as defined in [swsEdgeWeldConnectorSafetyFactorLiftOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEdgeWeldConnectorSafetyFactorLiftOption_e.html)

*DSafetyFactor*
:   Custom safety factor by which to reduce DWeldStrength; overrides the lift safety factor specified in NSafetyFactorLiftOption

*BIsEstimatedWeldSize*
:   True to calculate the appropriate size for the weld connector and compare it to DEstimatedWeldSize in the Weld Check Plot; false to just use DEstimatedWeldSize

*DEstimatedWeldSize*
:   Estimated weld size

*NEstimatedWeldSizeUnit*
:   DEstimatedWeldSize units as defined in [swsEstimatedWeldSizeUnits\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEstimatedWeldSizeUnits_e.html)

Sets the American Standard settings for weld sizing calculations.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetWeldSizingSettingUS( _    ByVal NElectrodeMaterial As System.Integer, _    ByVal DWeldStrength As System.Double, _    ByVal NWeldStrengthUnit As System.Integer, _    ByVal NSafetyFactorLiftOption As System.Integer, _    ByVal DSafetyFactor As System.Double, _    ByVal BIsEstimatedWeldSize As System.Boolean, _    ByVal DEstimatedWeldSize As System.Double, _    ByVal NEstimatedWeldSizeUnit As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWEdgeWeldConnector Dim NElectrodeMaterial As System.Integer Dim DWeldStrength As System.Double Dim NWeldStrengthUnit As System.Integer Dim NSafetyFactorLiftOption As System.Integer Dim DSafetyFactor As System.Double Dim BIsEstimatedWeldSize As System.Boolean Dim DEstimatedWeldSize As System.Double Dim NEstimatedWeldSizeUnit As System.Integer Dim value As System.Integer   value = instance.SetWeldSizingSettingUS(NElectrodeMaterial, DWeldStrength, NWeldStrengthUnit, NSafetyFactorLiftOption, DSafetyFactor, BIsEstimatedWeldSize, DEstimatedWeldSize, NEstimatedWeldSizeUnit) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetWeldSizingSettingUS(     System.int NElectrodeMaterial,    System.double DWeldStrength,    System.int NWeldStrengthUnit,    System.int NSafetyFactorLiftOption,    System.double DSafetyFactor,    System.bool BIsEstimatedWeldSize,    System.double DEstimatedWeldSize,    System.int NEstimatedWeldSizeUnit ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetWeldSizingSettingUS(  &   System.int NElectrodeMaterial, &   System.double DWeldStrength, &   System.int NWeldStrengthUnit, &   System.int NSafetyFactorLiftOption, &   System.double DSafetyFactor, &   System.bool BIsEstimatedWeldSize, &   System.double DEstimatedWeldSize, &   System.int NEstimatedWeldSizeUnit ) ``` | |

#### Parameters

*NElectrodeMaterial*
:   Electrode material as defined in [swsElectrodeMaterialTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsElectrodeMaterialTypes_e.html)

*DWeldStrength*
:   Ultimate shear strength of NElectrodeMaterial; if NElectrodeMaterial is swsElectrodeMaterialTypes\_e.swsElectrodeMaterialCustomAl or swsElectrodeMaterialTypes\_e.swsElectrodeMaterialCustomSteel, ultimate shear strength for the weld throat

*NWeldStrengthUnit*
:   DWeldStrength units as defined in [swsWeldStrengthUnits\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsWeldStrengthUnits_e.html)

*NSafetyFactorLiftOption*
:   Lift safety factor by which to reduce DWeldStrength as defined in [swsEdgeWeldConnectorSafetyFactorLiftOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEdgeWeldConnectorSafetyFactorLiftOption_e.html)

*DSafetyFactor*
:   Custom safety factor by which to reduce DWeldStrength; overrides the lift safety factor specified in NSafetyFactorLiftOption

*BIsEstimatedWeldSize*
:   True to calculate the appropriate size for the weld connector and compare it to DEstimatedWeldSize in the Weld Check Plot; false to just use DEstimatedWeldSize

*DEstimatedWeldSize*
:   Estimated weld size

*NEstimatedWeldSizeUnit*
:   DEstimatedWeldSize units as defined in [swsEstimatedWeldSizeUnits\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEstimatedWeldSizeUnits_e.html)

#### Return Value

Error code as defined in [swsWeldResultErrorCode\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsWeldResultErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWEdgeWeldConnector::SetWeldSizingSettingUS.

# ![](dotnetimages/collapse.gif)Example

See the [ICWEdgeWeldConnector](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWEdgeWeldConnector::GetCodeType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWEdgeWeldConnector~GetCodeType.html) returns [swsEdgeWeldSolverCode\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEdgeWeldSolverCode_e.html).swsEdgeWeldSolverCodeAWS.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWEdgeWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html)

[ICWEdgeWeldConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector_members.html)

[ICWEdgeWeldConnector::GetWeldSizingSettingUS Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~GetWeldSizingSettingUS.html)

[ICWEdgeWeldConnector::SetWeldSizingSettingEuro Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~SetWeldSizingSettingEuro.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0