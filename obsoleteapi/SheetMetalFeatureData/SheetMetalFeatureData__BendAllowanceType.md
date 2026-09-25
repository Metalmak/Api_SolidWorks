<!-- source: obsoleteapi/SheetMetalFeatureData/SheetMetalFeatureData__BendAllowanceType.htm -->

# SheetMetalFeatureData::BendAllowanceType

This
property is obsolete and has been superseded by SheetMetalFeatureData::GetCustomBendAllowance
and SheetMetalFeatureData::SetCustomBendAllowance.

Description

This property gets or sets the sheet metal
bend allowance type

Syntax (OLE Automation)

bendAllowanceType = SheetMetalFeatureData.BendAllowanceType  (VB
Get Property)

SheetMetalFeatureData.BendAllowanceType = bendAllowanceType  (VB
Set Property)

bendAllowanceType = SheetMetalFeatureData.GetBendAllowanceType (VB
Get Property)

SheetMetalFeatureData.SetBendAllowanceType = bendAllowanceType
 (VB Set Property)

|  |  |  |
| --- | --- | --- |
| Return: | (long) bendAllowanceType | Bend allowance type as defined in swBendAllowanceTypes\_e |

Syntax (COM)

status = SheetMetalFeatureData->get\_BendAllowanceType(&bendAllowanceType) (
COM Get Property)

status = SheetMetalFeatureData->put\_BendAllowanceType(bendAllowanceType) (
COM Get Property)

|  |  |  |
| --- | --- | --- |
| Output: | (long) bendAllowanceType | Bend allowance type as defined in swBendAllowanceTypes\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks