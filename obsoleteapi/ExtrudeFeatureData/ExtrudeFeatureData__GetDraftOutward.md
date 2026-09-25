<!-- source: obsoleteapi/ExtrudeFeatureData/ExtrudeFeatureData__GetDraftOutward.htm -->

# ExtrudeFeatureData::GetDraftOutward

This
method is obsolete and has been superseded by ExtrudeFeatureData2::GetDraftOutward.

Description

This method gets whether the extrusion feature
is drafted outward in forward or reverse direction

Syntax (OLE Automation)

draftOutward = ExtrudeFeatureData.GetDraftOutward
( forward )

|  |  |  |
| --- | --- | --- |
| Input: | (BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Return: | (BOOL) draftOutward | TRUE if feature is drafted outward, FALSE if not |

Syntax (COM)

status = ExtrudeFeatureData->GetDraftOutward (
forward, &draftOutward )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Output: | (VARIANT\_BOOL)draftOutward | TRUE if feature is drafted outward, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks