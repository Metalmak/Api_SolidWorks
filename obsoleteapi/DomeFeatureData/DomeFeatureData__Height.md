<!-- source: obsoleteapi/DomeFeatureData/DomeFeatureData__Height.htm -->

# DomeFeatureData::Height

This property is obsolete and has been
superseded by DomeFeatureData2::Height.

Description

This property controls the height of the dome.

Syntax (OLE Automation)

Height=
DomeFeatureData.Height (VB Get property)

DomeFeatureData.Height=
Height (VB Set property)

Height=
DomeFeatureData.GetHeight ( ) (C++ Get property)

DomeFeatureData.SetHeight
( Height) (C++ Set property)

| Property: | (double) Height | Height of the dome |

Syntax (COM)

status
= DomeFeatureData-> get\_Height( &Height)

status
= DomeFeatureData-> put\_Height( Height)

| Property: | (double) Height | Height of the dome |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This property does not affect geometry until you call Feature::ModifyDefinition.