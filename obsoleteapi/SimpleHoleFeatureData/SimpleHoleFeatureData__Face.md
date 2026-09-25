<!-- source: obsoleteapi/SimpleHoleFeatureData/SimpleHoleFeatureData__Face.htm -->

# SimpleHoleFeatureData::Face

This
property is obsolete and has been superseded by SimpleHoleFeatureData2::Face.

Description

This property gets or sets the simple hole
feature end condition face.

Syntax (OLE Automation)

face = SimpleHoleFeatureData.Face   (VB
Get property)

SimpleHoleFeatureData.Face = face   (VB
Set property)

face
= SimpleHoleFeatureData.GetFace ( )  (C++ Get property)

SimpleHoleFeatureData.SetFace ( face
)  (C++ Set property)

| Property: | (LPDISPATCH) face | Pointer to a dispatch object, the end condition face or NULL if the operation fails |

Syntax (COM)

status = SimpleHoleFeatureData ->get\_IFace ( &face )

status = SimpleHoleFeatureData ->put\_IFace ( face )

| Property: | (LPFACE) face | Pointer to a dispatch object, the end condition face or NULL if the operation fails |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Call SimpleHoleFeatureData::AccessSelections before using this property.