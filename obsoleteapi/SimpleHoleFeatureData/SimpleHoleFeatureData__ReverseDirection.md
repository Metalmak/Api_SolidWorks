<!-- source: obsoleteapi/SimpleHoleFeatureData/SimpleHoleFeatureData__ReverseDirection.htm -->

# SimpleHoleFeatureData::ReverseDirection

This property is obsolete and has been superseded
by SimpleHoleFeatureData2::ReverseDirection.

Description

This property gets or sets
whether the direction of the cut is reversed.

Syntax (OLE Automation)

reverseDirection = SimpleHoleFeatureData.ReverseDirection  (VB
Get property)

SimpleHoleFeatureData.ReverseDirection = reverseDirection  (VB Set property)

reverseDirection = SimpleHoleFeatureData.GetReverseDirection (
)  (C++ Get property)

SimpleHoleFeatureData.SetReverseDirection ( reverseDirection )  (C++ Set property)

| Property: | (BOOL) reverseDirection | TRUE if the direction of the cut should be reversed, FALSE if not |

Syntax (COM)

status = SimpleHoleFeatureData ->get\_ReverseDirection
( &reverseDirection )

status = SimpleHoleFeatureData ->put\_ReverseDirection
( reverseDirection )

| Property: | (VARIANT\_BOOL) reverseDirection | TRUE if the direction of the cut should be reversed, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks