<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager~SetResistanceValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetResistanceValue Method (ICWMultipleContactSetsEditManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMultipleContactSetsEditManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager.html) : SetResistanceValue Method (ICWMultipleContactSetsEditManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DResistanceValue*
:   Thermal resistance value

Sets the thermal resistance value for the contact sets to edit.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetResistanceValue( _    ByVal DResistanceValue As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMultipleContactSetsEditManager Dim DResistanceValue As System.Double Dim value As System.Integer   value = instance.SetResistanceValue(DResistanceValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetResistanceValue(     System.double DResistanceValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetResistanceValue(  &   System.double DResistanceValue ) ``` | |

#### Parameters

*DResistanceValue*
:   Thermal resistance value

#### Return Value

Error code as defined in [swsMultipleContactsEditErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMultipleContactsEditErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMultipleContactSetsEditManager::SetResistanceValue.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only for thermal studies and if [ICWMultipleContactSetsEditManager::SetContactType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager~SetContactType.html) sets [swsContactSetTypeThermal\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactSetTypeThermal_e.html).swsContactSetTypeThermalResistance.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMultipleContactSetsEditManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager.html)

[ICWMultipleContactSetsEditManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager_members.html)

[ICWMultipleContactSetsEditManager::SetResistanceType Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager~SetResistanceType.html)

[ICWMultipleContactSetsEditManager::SetResistanceUnitSystem Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager~SetResistanceUnitSystem.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0