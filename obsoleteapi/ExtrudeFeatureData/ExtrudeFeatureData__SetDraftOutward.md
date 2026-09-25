<!-- source: obsoleteapi/ExtrudeFeatureData/ExtrudeFeatureData__SetDraftOutward.htm -->

# ExtrudeFeatureData::SetDraftOutward

This
method is obsolete and has been superseded by ExtrudeFeatureData2::SetDraftOutward.

Description

This method sets whether the extrusion feature
should draft outward in forward or reverse direction.

Syntax (OLE Automation)

void ExtrudeFeatureData.SetDraftOutward ( forward, draftOutward )

| Input: | (BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Input: | (BOOL) draftOutward | TRUE if feature is drafted outward, FALSE if not |

Syntax (COM)

status = ExtrudeFeatureData->SetDraftOutward (
forward, draftOutward )

| Input: | (VARIANT\_BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Input: | (VARIANT\_BOOL) draftOutward | TRUE if feature is drafted outward, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks