<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager~SetResistanceType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetResistanceType Method (ICWMultipleContactSetsEditManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMultipleContactSetsEditManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager.html) : SetResistanceType Method (ICWMultipleContactSetsEditManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NResistanceType*
:   Thermal resistance type as defined in [swsResistanceType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResistanceType_e.html)

Sets the thermal resistance type for the contact sets to edit.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetResistanceType( _    ByVal NResistanceType As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMultipleContactSetsEditManager Dim NResistanceType As System.Integer Dim value As System.Integer   value = instance.SetResistanceType(NResistanceType) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetResistanceType(     System.int NResistanceType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetResistanceType(  &   System.int NResistanceType ) ``` | |

#### Parameters

*NResistanceType*
:   Thermal resistance type as defined in [swsResistanceType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResistanceType_e.html)

#### Return Value

Error code as defined in [swsMultipleContactsEditErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMultipleContactsEditErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMultipleContactSetsEditManager::SetResistanceType.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only for thermal studies and if [ICWMultipleContactSetsEditManager::SetContactType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager~SetContactType.html) sets [swsContactSetTypeThermal\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactSetTypeThermal_e.html).swsContactSetTypeThermalResistance.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMultipleContactSetsEditManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager.html)

[ICWMultipleContactSetsEditManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager_members.html)

[ICWMultipleContactSetsEditManager::SetResistanceUnitSystem Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager~SetResistanceUnitSystem.html)

[ICWMultipleContactSetsEditManager::SetResistanceValue Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager~SetResistanceValue.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0