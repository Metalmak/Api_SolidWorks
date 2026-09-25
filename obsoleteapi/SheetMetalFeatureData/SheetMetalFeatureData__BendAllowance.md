<!-- source: obsoleteapi/SheetMetalFeatureData/SheetMetalFeatureData__BendAllowance.htm -->

# SheetMetalFeatureData::BendAllowance

This
property is obsolete and has been superseded by SheetMetalFeatureData::GetCustomBendAllowance
and SheetMetalFeatureData::SetCustomBendAllowance.

Description

This property gets or set the bend allowance
for this sheet metal feature.

Syntax (OLE Automation)

bendAllowance = SheetMetalFeatureData.BendAllowance  (
VB Get Property )

SheetMetalFeatureData.BendAllowance = bendAllowance  (
VB Set Property )

bendAllowance = SheetMetalFeatureData.GetBendAllowance (
C++ Get Property )

SheetMetalFeatureData.SetBendAllowance = bendAllowance (
C++ Set Property )

|  |  |  |
| --- | --- | --- |
| Return: | (double) bendAllowance | Value that describes the bend allowance |

Syntax (COM)

status = SheetMetalFeatureData->get\_BendAllowance
( &bendAllowance) ( COM Get Property )

status = SheetMetalFeatureData->put\_BendAllowance
( bendAllowance)   (
COM Set Property )

|  |  |  |
| --- | --- | --- |
| Output: | (double) bendAllowance | Value that describes the bend allowance |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks