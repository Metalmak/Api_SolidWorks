<!-- source: obsoleteapi/ExtrudeFeatureData/ExtrudeFeatureData__GetDraftWhileExtruding.htm -->

# ExtrudeFeatureData::GetDraftWhileExtruding

This
method is obsolete and has been superseded by ExtrudeFeatureData2::GetDraftWhileExtruding.

Description

This method gets whether the feature is drafted
while extruding in forward or reverse direction.

Syntax (OLE Automation)

draftWhileExtrude = ExtrudeFeatureData.GetDraftWhileExtruding
( forward )

| Input: | (BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Return: | (BOOL) draftWhileExtrude | TRUE if feature is drafted while extruding, FALSE if not |

Syntax (COM)

status = ExtrudeFeatureData->GetDraftWhileExtruding
( forward, &draftWhileExtrude )

| Input: | (VARIANT\_BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Output: | (VARIANT\_BOOL) draftWhileExtrude | TRUE if feature is drafted while extruding, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks