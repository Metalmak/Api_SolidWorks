<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__Diameter.htm -->

# WizardHoleFeatureData::Diameter

This
property is obsolete and has been superseded by WizardHoleFeatureData2::Diameter.

Description

This property gets or sets the hole wizard
feature hole diameter.

Syntax (OLE Automation)

diameter = WizardHoleFeatureData.Diameter   (VB
Get property)

WizardHoleFeatureData.Diameter = diameter   (VB
Set property)

diameter = WizardHoleFeatureData.GetDiameter ( )  (C++
Get property)

WizardHoleFeatureData.SetDiameter ( diameter )  (C++
Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (double) diameter | Hole diameter |

Syntax (COM)

status = WizardHoleFeatureData ->get\_Diameter
( &diameter )

status = WizardHoleFeatureData ->put\_Diameter
( diameter )

|  |  |  |
| --- | --- | --- |
| Property: | (double) diameter | Hole diameter |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This property is not relevant for tapered and
tapered drilled holes.