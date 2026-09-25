<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__MidCounterSinkAngle.htm -->

# WizardHoleFeatureData::MidCounterSinkAngle

This
property is obsolete and has been superseded by WizardHoleFeatureData2::MidCounterSinkAngle.

Description

This property gets or sets the hole wizard
feature middle counter sink angle.

Syntax (OLE Automation)

csinkAngle = WizardHoleFeatureData.MidCounterSinkAngle
  (VB Get property)

WizardHoleFeatureData.MidCounterSinkAngle = csinkAngle   (VB Set property)

csinkAngle = WizardHoleFeatureData.GetMidCounterSinkAngle
( )  (C++ Get property)

WizardHoleFeatureData.SetMidCounterSinkAngle ( csinkAngle )  (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (double) csinkAngle | Middle counter sink angle |

Syntax (COM)

status = WizardHoleFeatureData ->get\_MidCounterSinkAngle
( &csinkAngle )

status = WizardHoleFeatureData ->put\_MidCounterSinkAngle
( csinkAngle )

|  |  |  |
| --- | --- | --- |
| Property: | (double) csinkAngle | Middle counter sink angle |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This property is relevant only for counter- sink
and counter- sink drilled holes.