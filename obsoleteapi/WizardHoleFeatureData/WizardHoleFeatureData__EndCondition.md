<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__EndCondition.htm -->

# WizardHoleFeatureData::EndCondition

This
property is obsolete and has been superseded by WizardHoleFeatureData2::EndCondition.

Description

This property gets or sets the hole wizard
feature end condition type.

Syntax (OLE Automation)

endCondition = WizardHoleFeatureData.EndCondition   (VB
Get property)

WizardHoleFeatureData.EndCondition = EndCondition   (VB Set property)

endCondition = WizardHoleFeatureData.GetEndCondition ( )  (C++
Get property)

WizardHoleFeatureData.SetEndCondition ( endCondition )   (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (int) endCondition | End condition type of the hole wizard feature |

Syntax (COM)

status = WizardHoleFeatureData ->get\_EndCondition
( &endCondition )

status = WizardHoleFeatureData ->put\_EndCondition
( endCondition )

|  |  |  |
| --- | --- | --- |
| Property: | (int) endCondition | End condition type of the hole wizard feature |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The end condition type is specified in swEndConditions\_e. It should
have one of these values:

* swEndCondBlind
* swEndCondThroughAll
* swEndCondThroughNext
* swEndCondUpToVertex
* swEndCondUpToSurface
* swEndCondOffsetFromSurface
* swEndCondMidPlane