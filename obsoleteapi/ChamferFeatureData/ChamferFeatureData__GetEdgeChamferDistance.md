<!-- source: obsoleteapi/ChamferFeatureData/ChamferFeatureData__GetEdgeChamferDistance.htm -->

# ChamferFeatureData::GetEdgeChamferDistance

This method is obsolete and has been superseded
by ChamferFeatureData2::GetEdgeChamferDistance.

Description

This method gets the edge chamfer distance
on either side of the edge.

Syntax (OLE Automation)

distance = ChamferFeatureData.GetEdgeChamferDistance
( side )

| Input: | (int) side | Feature direction, set to 0 or 1; for angle-distance chamfer, set to 0 |
| Return: | (double) distance | Edge chamfer distance |

Syntax (COM)

status = ChamferFeatureData ->GetEdgeChamferDistance
( side, &distance
)

| Input: | (int) side | Feature direction, set to 0 or 1; for angle-distance chamfer, set to 0 |
| Output:: | (double) distance | Edge chamfer distance. |
| Return: | (HRESULT) status | S\_OK if successful. |

Remarks