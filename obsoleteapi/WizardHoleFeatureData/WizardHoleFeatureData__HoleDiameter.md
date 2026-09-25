<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__HoleDiameter.htm -->

# WizardHoleFeatureData::HoleDiameter

This
property is obsolete and has been superseded by WizardHoleFeatureData2::HoleDiameter.

Description

This property gets or sets the hole wizard
feature hole diameter.

Syntax (OLE Automation)

diameter = WizardHoleFeatureData.HoleDiameter   (VB
Get property)

WizardHoleFeatureData.HoleDiameter = diameter   (VB
Set property)

diameter = WizardHoleFeatureData.GetHoleDiameter
( )  (C++ Get property)

WizardHoleFeatureData.SetHoleDiameter ( diameter
)  (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (double) diameter | Hole diameter |

Syntax (COM)

status = WizardHoleFeatureData ->get\_HoleDiameter
( &diameter )

status = WizardHoleFeatureData ->put\_HoleDiameter
( diameter )

|  |  |  |
| --- | --- | --- |
| Property: | (double) diameter | Hole diameter |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This property is not relevant for tapered and
tapered drilled holes.