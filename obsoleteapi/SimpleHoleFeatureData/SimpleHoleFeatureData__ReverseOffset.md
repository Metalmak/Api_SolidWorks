<!-- source: obsoleteapi/SimpleHoleFeatureData/SimpleHoleFeatureData__ReverseOffset.htm -->

# SimpleHoleFeatureData::ReverseOffset

This
property is obsolete and has been superseded by SimpleHoleFeatureData2::ReverseOffset.

Description

This property gets or sets whether the offset
from the surface should be reversed.

Syntax (OLE Automation)

reverseOffset = SimpleHoleFeatureData.ReverseOffset  (VB
Get property)

SimpleHoleFeatureData.ReverseOffset = reverseOffset  (VB Set property)

reverseOffset = SimpleHoleFeatureData.GetReverseOffset ( ) (C++
Get property)

SimpleHoleFeatureData.SetReverseOffset (reverseOffset)  (C++ Set property)

| Property: | (BOOL) reverseOffset | TRUE if the offset from the surface should be reversed, FALSE if not |

Syntax (COM)

status = SimpleHoleFeatureData ->get\_ReverseOffset
( &reverseOffse t)

status = SimpleHoleFeatureData ->put\_ReverseOffset
( reverseOffset )

| Property: | (VARIANT\_BOOL) reverseOffset | TRUE if the offset from the surface should be reversed, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks