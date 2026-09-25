<!-- source: obsoleteapi/BendsFeatureData/BendsFeatureData__BendAllowance.htm -->

# BendsFeatureData::BendAllowance

This property is obsolete and has been superseded
by BendsFeatureData::GetCustomBendAllowance
and BendsFeatureData::SetCustomBendAllowance.

Description

This property gets or sets the bend allowance
for this Flatten-Bends/Process-Bends feature.

Syntax (OLE Automation)

bendAllowance = BendsFeatureData.BendAllowance  (
VB Get Property )

BendsFeatureData.BendAllowance = bendAllowance  (
VB Set Property )

bendAllowance = BendsFeatureData.GetBendAllowance  (
C++ Get Property )

BendsFeatureData.SetBendAllowance = bendAllowance  (
C++ Set Property )

|  |  |  |
| --- | --- | --- |
| Return: | (double) bendAllowance | Value for the bend allowance |

Syntax (COM)

status = BendsFeatureData->get\_BendAllowance (
&bendAllowance) ( COM Get Property )

status = BendsFeatureData->put\_BendAllowance (
&bendAllowance) ( COM Set Property )

|  |  |  |
| --- | --- | --- |
| Output: | (double) bendAllowance | Value for the bend allowance |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks