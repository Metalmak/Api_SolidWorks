<!-- source: obsoleteapi/RevolveFeatureData/RevolveFeatureData__GetWallThickness.htm -->

# RevolveFeatureData::GetWallThickness

This
method is obsolete and has been superseded by RevolveFeatureData2::GetWallThickness.

Description

This method gets the wall thickness of the
thin revolution feature in forward or reverse direction.

Syntax (OLE Automation)

wallThickness = RevolveFeatureData.GetWallThickness
( forward )

|  |  |  |
| --- | --- | --- |
| Input: | (BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Return: | (double) wallThickness | Wall thickness |

Syntax (COM)

status = RevolveFeatureData ->GetWallThickness
( forward, &wallThickness )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Output: | (double) wallThickness | Wall thickness |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Relevant only for thin features.