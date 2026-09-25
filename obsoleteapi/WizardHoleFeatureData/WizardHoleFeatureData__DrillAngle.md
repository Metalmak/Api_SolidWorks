<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__DrillAngle.htm -->

# WizardHoleFeatureData::DrillAngle

This property is obsolete and has been superseded
by WizardHoleFeatureData2::DrillAngle.

Description

This property gets or sets the hole wizard
feature drill angle.

Syntax (OLE Automation)

drillAngle = WizardHoleFeatureData.DrillAngle   (VB
Get property)

WizardHoleFeatureData.DrillAngle = drillAngle   (VB Set property)

drillAngle = WizardHoleFeatureData.GetDrillAngle
( )  (C++ Get property)

WizardHoleFeatureData.SetDrillAngle ( drillAngle )   (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (double) drillAngle | Drill angle |

Syntax (COM)

status = WizardHoleFeatureData ->get\_DrillAngle
( &drillAngle )

status = WizardHoleFeatureData ->put\_DrillAngle
( drillAngle )

|  |  |  |
| --- | --- | --- |
| Property: | (double) drillAngle | Drill angle |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This property is relevant only for simple drilled,
tapered drilled, counter-bore drilled, counter-sunk drilled and counter-drilled
drilled holes.