<!-- source: obsoleteapi/ExtrudeFeatureData/ExtrudeFeatureData__GetDepth.htm -->

# ExtrudeFeatureData::GetDepth

This
method is obsolete and has been superseded by ExtrudeFeatureData2::GetDepth.

Description

This method gets the depth of the extrusion
feature in the forward or reverse direction.

Syntax (OLE Automation)

depth = ExtrudeFeatureData.GetDepth
( forward )

|  |  |  |
| --- | --- | --- |
| Input: | (BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Return: | (double) depth | Depth of the extrusion |

Syntax (COM)

status = ExtrudeFeatureData->GetDepth ( forward,
&depth )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Output:: | (double) depth | Depth of the extrusion |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks