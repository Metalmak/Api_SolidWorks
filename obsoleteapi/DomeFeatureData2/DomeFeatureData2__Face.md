<!-- source: obsoleteapi/DomeFeatureData2/DomeFeatureData2__Face.htm -->

# DomeFeatureData2::Face

This property is obsolete and has been superseded
by DomeFeatureData2::Faces,
DomeFeatureData2::IGetFaces,
and DomeFeatureData2::ISetFaces.

Description

This
property gets or sets the planar face associated with this dome feature.

Syntax (OLE Automation)

Set
Face= DomeFeatureData2.Face (VB Get property)

Set
DomeFeatureData2.Face= Face (VB Set property)

Face=
DomeFeatureData2.GetFace ( ) (C++ Get property)

DomeFeatureData2.SetFace
( Face) (C++ Set property)

| Property: | (LPDISPATCH) Face | Dispatch pointer for the face associated with the dome |

Syntax (COM)

status
= DomeFeatureData2-> get\_IFace( &face)

status
= DomeFeatureData2-> put\_IFace( face)

| Property: | (LPFACE2) face | Pointer to the face associated with the dome |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This property does not affect geometry until you call Feature::ModifyDefinition.

See Accessing Selections that Define Features
for additional details on using this property.