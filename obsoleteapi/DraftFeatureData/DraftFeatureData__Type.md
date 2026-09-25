<!-- source: obsoleteapi/DraftFeatureData/DraftFeatureData__Type.htm -->

# DraftFeatureData::Type

This property is obsolete and has been
superseded by DraftFeatureData2::Type.

Description

This property gets the draft feature type.

Syntax (OLE Automation)

type = DraftFeatureData.Type   (VB
Get property)

type
= DraftFeatureData.GetType ( )  (C++ Get property)

| Property: | (int) type | Draft type:   * 0 = Neutral   Plane * 1 = Parting Line |

Syntax (COM)

status = DraftFeatureData ->get\_Type ( & type )

| Property: | (int) type | Draft type:   * 0 = Neutral   Plane * 1 = Parting Line |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This is a read-only property.