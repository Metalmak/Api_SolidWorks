<!-- source: obsoleteapi/SimpleFilletFeatureData/SimpleFilletFeatureData__RoundCorners.htm -->

# SimpleFilletFeatureData::RoundCorners

This
property is obsolete and has been superseded by SimpleFilletFeatureData2::RoundCorners.

Description

This property gets or sets whether the simple
fillet feature has round corners.

Syntax (OLE Automation)

roundCorners = SimpleFilletFeatureData.RoundCorners  (VB
Get property)

SimpleFilletFeatureData.RoundCorners = roundCorners  (VB Set property)

roundCorners = SimpleFilletFeatureData.GetRoundCorners ( ) (C++
Get property)

SimpleFilletFeatureData.SetRoundCorners ( roundCorners ) (C++ Set property)

| Property: | (BOOL) roundCorners | TRUE if simple fillet feature has round corners, FALSE if not |

Syntax (COM)

status = SimpleFilletFeatureData ->get\_RoundCorners
( &roundCorners )

status = SimpleFilletFeatureData ->put\_RoundCorners
( roundCorners )

| Property: | (VARIANT\_BOOL) roundCorners | TRUE if simple fillet feature has round corners, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks