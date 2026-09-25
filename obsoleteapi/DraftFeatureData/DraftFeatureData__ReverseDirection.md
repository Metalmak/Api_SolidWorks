<!-- source: obsoleteapi/DraftFeatureData/DraftFeatureData__ReverseDirection.htm -->

# DraftFeatureData::ReverseDirection

This property is obsolete and has been
superseded by DraftFeatureData2::ReverseDirection.

Description

This property gets or sets whether to reverse
the direction of the draft feature.

Syntax (OLE Automation)

reverseDirection = DraftFeatureData.ReverseDirection  (VB
Get property)

DraftFeatureData.ReverseDirection = reverseDirection  (VB Set property)

reverseDirection = DraftFeatureData.GetReverseDirection ( ) (C++
Get property)

DraftFeatureData.SetReverseDirection ( reverseDirection )  (C++ Set property)

| Property: | (BOOL) reverseDirection | TRUE if the direction of the draft feature is reversed, FALSE if it is not |

Syntax (COM)

status = DraftFeatureData ->get\_ReverseDirection
( &reverseDirection )

status = DraftFeatureData ->put\_ReverseDirection
( reverseDirection )

| Property: | (VARIANT\_BOOL) reverseDirection | TRUE if the direction of the draft feature is reversed, FALSE if it is not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks