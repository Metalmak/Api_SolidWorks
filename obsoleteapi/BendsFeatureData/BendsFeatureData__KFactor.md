<!-- source: obsoleteapi/BendsFeatureData/BendsFeatureData__KFactor.htm -->

# BendsFeatureData::KFactor

This property is obsolete and has been
superseded by BendsFeatureData::GetCustomBendAllowance
and BendsFeatureData::SetCustomBendAllowance.

Description

This property gets or sets the K-Factor for
this Flatten-Bends/Process-Bends feature.

Syntax (OLE Automation)

kFactor = BendsFeatureData.KFactor  ( VB
Get Property )

BendsFeatureData.KFactor = kFactor  ( VB
Set Property )

kFactor = BendsFeatureData.GetKFactor  (
C++ Get Property )

BendsFeatureData.SetKFactor = kFactor  (
C++ Set Property )

| Return: | (double) kFactor | Value of the K factor |

Syntax (COM)

status = BendsFeatureData->get\_KFactor ( &kFactor
)  ( COM Get Property )

status = BendsFeatureData->put\_KFactor ( kFactor
)  ( COM Set Property )

| Output: | (double) kFac | Value of the K factor |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks