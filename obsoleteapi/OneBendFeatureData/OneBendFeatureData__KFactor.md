<!-- source: obsoleteapi/OneBendFeatureData/OneBendFeatureData__KFactor.htm -->

# OneBendFeatureData::KFactor

This property is obsolete and has been
superseded by OneBendFeatureData::GetCustomBendAllowance
and OneBendFeatureData::SetCustomBendAllowance.

Description

This property gets or sets the K-Factor for
this bend.

Syntax (OLE Automation)

kFactor = OneBendFeatureData.KFactor  (
VB Get Property )

OneBendFeatureData.KFactor = kFactor  (
VB Set Property )

kFactor = OneBendFeatureData.GetKFactor  (
C++ Get Property )

OneBendFeatureData.SetKFactor = kFactor  (
C++ Set Property )

|  |  |  |
| --- | --- | --- |
| Return: | (double) kFactor | Value of the K-Factor |

Syntax (COM)

status = OneBendFeatureData->get\_KFactor (&kFactor)  (COM
Get Property )

status = OneBendFeatureData->put\_KFactor ( kFactor)  (COM
Set Property )

|  |  |  |
| --- | --- | --- |
| Output: | (double) kFactor | Value of the K-Factor |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks