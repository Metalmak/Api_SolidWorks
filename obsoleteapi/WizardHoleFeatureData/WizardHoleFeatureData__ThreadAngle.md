<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__ThreadAngle.htm -->

# WizardHoleFeatureData::ThreadAngle

This
property is obsolete and has been superseded by WizardHoleFeatureData2::ThreadAngle.

Description

This property gets or sets the hole wizard
feature thread angle.

Syntax (OLE Automation)

threadAngle = WizardHoleFeatureData.ThreadAngle
  (VB Get property)

WizardHoleFeatureData.ThreadAngle = threadAngle   (VB Set property)

threadAngle = WizardHoleFeatureData.GetThreadAngle
( )  (C++ Get property)

WizardHoleFeatureData.SetThreadAngle ( threadAngle )  (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (double) threadAngle | Thread angle |

Syntax (COM)

status = WizardHoleFeatureData ->get\_ThreadAngle
( &threadAngle )

status = WizardHoleFeatureData ->put\_ThreadAngle
( threadAngle )

|  |  |  |
| --- | --- | --- |
| Property: | (double) threadAngle | Thread angle |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This property is relevant only threaded holes.