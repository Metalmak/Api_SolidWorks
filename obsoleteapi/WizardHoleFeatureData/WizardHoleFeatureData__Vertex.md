<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__Vertex.htm -->

# WizardHoleFeatureData::Vertex

This
property is obsolete and has been superseded by WizardHoleFeatureData2::Vertex.

Description

This propery gets or sets the hole wizard feature
end condition vertex.

Syntax (OLE Automation)

vertex = WizardHoleFeatureData.Vertex   (VB
Get property)

WizardHoleFeatureData.Vertex = vertex   (VB
Set property)

vertex
= WizardHoleFeatureData.GetVertex ( )  (C++ Get property)

WizardHoleFeatureData.SetVertex ( vertex )   (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (LPDISPATCH) vertex | Pointer to a dispatch object, the end condition vertex, or NULL if the operation fails |

Syntax (COM)

status = WizardHoleFeatureData ->get\_IVertex (
&vertex )

status = WizardHoleFeatureData ->put\_IVertex (
vertex )

|  |  |  |
| --- | --- | --- |
| Property: | (LPVERTEX) vertex | Pointer to the end condition Vertex object or NULL if the operation fails |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Call WizardHoleFeatureData::AccessSelections before using this property.