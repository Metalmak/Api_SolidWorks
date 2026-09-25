<!-- source: obsoleteapi/SimpleHoleFeatureData/SimpleHoleFeatureData__Vertex.htm -->

# SimpleHoleFeatureData::Vertex

This
property is obsolete and has been superseded by SimpleHoleFeatureData2::Vertex.

Description

This property gets or sets the simple hole
feature end condition vertex.

Syntax (OLE Automation)

vertex = SimpleHoleFeatureData.Vertex   (VB
Get property)

SimpleHoleFeatureData.Vertex = vertex   (VB
Set property)

vertex
= SimpleHoleFeatureData.GetVertex ( )  (C++ Get property)

SimpleHoleFeatureData.SetVertex ( vertex )  (C++ Set property)

| Property: | (LPDISPATCH) vertex | Pointer to a dispatch object, the end condition vertex or NULL if the operation fails |

Syntax (COM)

status = WizardHoleFeatureData ->get\_IVertex (
&vertex )

status = WizardHoleFeatureData ->put\_IVertex (
vertex )

| Property: | (LPVERTEX) vertex | Pointer to a dispatch object, the end condition vertex or NULL if the operation fails |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Call SimpleHoleFeatureData::AccessSelections before using this property.