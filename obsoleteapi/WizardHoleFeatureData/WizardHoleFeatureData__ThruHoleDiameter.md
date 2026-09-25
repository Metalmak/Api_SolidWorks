<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__ThruHoleDiameter.htm -->

# WizardHoleFeatureData::ThruHoleDiameter

This
property is obsolete and has been superseded by WizardHoleFeatureData2::ThruHoleDiameter.

Description

This property gets or sets the hole wizard
feature through hole diameter.

Syntax (OLE Automation)

diameter = WizardHoleFeatureData.ThruHoleDiameter
  (VB Get property)

WizardHoleFeatureData.ThruHoleDiameter = diameter  (VB
Set property)

diameter = WizardHoleFeatureData.GetThruHoleDiameter
( ) (C++ Get property)

WizardHoleFeatureData.SetThruHoleDiameter ( diameter
)  (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (double) diameter | Through hole diameter |

Syntax (COM)

status = WizardHoleFeatureData ->get\_ThruHoleDiameter
( &diameter )

status = WizardHoleFeatureData ->put\_ThruHoleDiameter
( diameter )

|  |  |  |
| --- | --- | --- |
| Property: | (double) diameter | Through hole diameter |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The property is not relevant for tapered and
tapered drilled holes.