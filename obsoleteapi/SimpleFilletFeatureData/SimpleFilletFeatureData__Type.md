<!-- source: obsoleteapi/SimpleFilletFeatureData/SimpleFilletFeatureData__Type.htm -->

# SimpleFilletFeatureData::Type

This
property is obsolete and has been superseded by SimpleFilletFeatureData2::Type.

Description

This property gets the simple fillet feature
type.

Syntax (OLE Automation)

type = SimpleFilletFeatureData.Type   (VB
Get property)

type
= SimpleFilletFeatureData.GetType ( )  (C++ Get property)

| Property: | (int) type | Type of fillet feature:   * 0 = Constant   radius * 1 = Variable radius * 2 = Face blend |

Syntax (COM)

status = SimpleFilletFeatureData ->get\_Type (
&type )

| Property: | (int) type | Type of fillet feature:   * 0 = Constant   radius * 1 = Variable radius * 2 = Face blend |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks