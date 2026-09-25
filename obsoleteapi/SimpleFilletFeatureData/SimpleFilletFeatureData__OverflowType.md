<!-- source: obsoleteapi/SimpleFilletFeatureData/SimpleFilletFeatureData__OverflowType.htm -->

# SimpleFilletFeatureData::OverflowType

This
property is obsolete and has been superseded by SimpleFilletFeatureData2::OverflowType.

Description

This property gets or sets the simple fillet
feature overflow type.

Syntax (OLE Automation)

overflowType = SimpleFilletFeatureData.OverflowType  (VB
Get property)

SimpleFilletFeatureData.OverflowType = overflowType  (VB Set property)

overflowType = SimpleFilletFeatureData.GetOverflowType ( ) (C++
Get property)

SimpleFilletFeatureData.SetOverflowType ( overflowType )  (C++ Set property)

| Property: | (int) overflowType | Overflow type of the simple fillet feature:   * 0 = Default * 1 = Keep edge * 2 = Keep surface |

Syntax (COM)

status = SimpleFilletFeatureData ->get\_OverflowType
( &overflowType )

status = SimpleFilletFeatureData ->put\_OverflowType
( overflowType )

| Property: | (int) overflowType | Overflow type of the simple fillet feature:   * 0 = Default * 1 = Keep edge * 2 = Keep surface |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks