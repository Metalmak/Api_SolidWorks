<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__ThreadDepth.htm -->

# WizardHoleFeatureData::ThreadDepth

This
property is obsolete and has been superseded by WizardHoleFeatureData2::ThreadDepth.

Description

This property gets or sets the hole wizard
feature thread depth.

Syntax (OLE Automation)

depth = WizardHoleFeatureData.ThreadDepth
  (VB Get property)

WizardHoleFeatureData.ThreadDepth = depth  (VB Set property)

depth
= WizardHoleFeatureData.GetThreadDepth ( )  (C++ Get
property)

WizardHoleFeatureData.SetThreadDepth ( depth )  (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (double) depth | Thread depth |

Syntax (COM)

status = WizardHoleFeatureData ->get\_ThreadDepth
( &depth )

status = WizardHoleFeatureData ->put\_ThreadDepth
( depth )

|  |  |  |
| --- | --- | --- |
| Property: | (double) depth | Thread depth |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks