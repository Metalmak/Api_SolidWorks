<!-- source: obsoleteapi/SimpleHoleFeatureData/SimpleHoleFeatureData__DraftWhileExtruding.htm -->

# SimpleHoleFeatureData::DraftWhileExtruding

This
property is obsolete and has been superseded by SimpleHoleFeatureData2::DraftWhileExtruding.

Description

This property gets or sets whether to draft
the simple hole feature while extruding.

Syntax (OLE Automation)

draftWhileExtrude = SimpleHoleFeatureData.DraftWhileExtruding  (VB
Get property)

SimpleHoleFeatureData.DraftWhileExtruding = draftWhileExtrude  (VB Set property)

draftWhileExtrude = SimpleHoleFeatureData.GetDraftWhileExtruding
( )  (C++ Get property)

SimpleHoleFeatureData.SetDraftWhileExtruding ( draftWhileExtrude )  (C++ Set property)

| Property: | (BOOL) draftWhileExtrude | TRUE if to draft the simple hole feature while extruding, FALSE if not |

Syntax (COM)

status = SimpleHoleFeatureData ->get\_DraftWhileExtruding
( &draftWhileExtrude )

status = SimpleHoleFeatureData ->put\_DraftWhileExtruding
( draftWhileExtrude )

| Property: | (VARIANT\_BOOL) draftWhileExtrude | TRUE if to draft the simple hole feature while extruding, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks