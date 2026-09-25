<!-- source: obsoleteapi/OneBendFeatureData/OneBendFeatureData__BendAllowance.htm -->

# OneBendFeatureData::BendAllowance

This property is obsolete and has been superseded
by OneBendFeatureData::GetCustomBendAllowance
and OneBendFeatureData::SetCustomBendAllowance.

Description

This property gets or sets the bend allowance
for this bend feature.

Syntax (OLE Automation)

bendAllowance = OneBendFeatureData.BendAllowance  (
VB Get Property )

OneBendFeatureData.BendAllowance = bendAllowance  (
VB Set Property )

bendAllowance = OneBendFeatureData.GetBendAllowance  (
C++ Get Property )

OneBendFeatureData.SetBendAllowance = bendAllowance  (
C++ Set Property )

|  |  |  |
| --- | --- | --- |
| Return: | (double) bendAllowance | Value of the bend allowance |

Syntax (COM)

status = OneBendFeatureData->get\_BendAllowance
( &bendAllowance) ( COM Get Property )

status = OneBendFeatureData->put\_BendAllowance
( &bendAllowance) ( COM Set Property )

|  |  |  |
| --- | --- | --- |
| Output: | (long) bendAllowance | Value of the bend allowance |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks