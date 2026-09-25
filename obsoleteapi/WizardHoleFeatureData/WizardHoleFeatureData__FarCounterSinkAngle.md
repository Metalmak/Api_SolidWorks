<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__FarCounterSinkAngle.htm -->

# WizardHoleFeatureData::FarCounterSinkAngle

This
property is obsolete and has been superseded by WizardHoleFeatureData2::FarCounterSinkAngle.

Description

This property gets or sets the hole wizard
feature far counter sink angle.

Syntax (OLE Automation)

csinkAngle = WizardHoleFeatureData.FarCounterSinkAngle   (VB
Get property)

WizardHoleFeatureData.FarCounterSinkAngle = csinkAngle   (VB Set property)

csinkAngle = WizardHoleFeatureData.GetFarCounterSinkAngle
( )  (C++ Get property)

WizardHoleFeatureData.SetFarCounterSinkAngle ( csinkAngle )  (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (double) csinkAngle | Far counter sink angle of the hole wizard feature |

Syntax (COM)

status = WizardHoleFeatureData ->get\_FarCounterSinkAngle
( &csinkAngle )

status = WizardHoleFeatureData ->put\_FarCounterSinkAngle
( csinkAngle )

|  |  |  |
| --- | --- | --- |
| Property: | (double) csinkAngle | Far counter sink angle of the hole wizard feature |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This property is relevant only for counter- sink
and counter- sink drilled holes.