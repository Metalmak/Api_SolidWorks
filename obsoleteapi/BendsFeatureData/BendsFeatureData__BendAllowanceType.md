<!-- source: obsoleteapi/BendsFeatureData/BendsFeatureData__BendAllowanceType.htm -->

# BendsFeatureData::BendAllowanceType

This
property is obsolete and has been superseded by BendsFeatureData::GetCustomBendAllowance
and BendsFeatureData::SetCustomBendAllowance.

Description

This property gets or sets the bend allowance
type for this Flatten-Bends/Process-Bends feature.

Syntax (OLE Automation)

bendAllowanceType = BendsFeatureData.BendAllowanceType  (
VB Get Property )

BendsFeatureData.BendAllowanceType = bendAllowanceType  (
VB Set Property )

bendAllowanceType = BendsFeatureData.GetBendAllowanceType  (
C++ Get Property )

BendsFeatureData.SetBendAllowanceType = bendAllowanceType  (
C++ Set Property )

| Return: | (long) bendAllowanceType | Bend allowance type as defined in swBendAllowanceTypes\_e |

Syntax (COM)

status = BendsFeatureData->get\_BendAllowanceType
( &bendAllowanceType) ( COM Get Property )

status = BendsFeatureData->put\_BendAllowanceType
( bendAllowanceType) ( COM Set Property )

| Output: | (long) bendAllowanceType | Bend allowance type as defined in swBendAllowanceTypes\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks