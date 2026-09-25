<!-- source: obsoleteapi/DomeFeatureData/DomeFeatureData__Elliptical.htm -->

# DomeFeatureData::Elliptical

This property is obsolete and has been
superseded by DomeFeatureData2::Elliptical.

Description

If the face on which the dome is defined is a circular or elliptical
face, then this flag controls whether the dome is a half ellipsoid, with
a height equal to one of the ellipsoid radii.

Syntax (OLE Automation)

Elliptical=
DomeFeatureData.Elliptical (VB Get property)

DomeFeatureData.Elliptical=
Elliptical (VB Set property)

Elliptical=
DomeFeatureData.GetElliptical ( ) (C++ Get property)

DomeFeatureData.SetElliptical
( Elliptical) (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (BOOL) Elliptical | TRUE if the dome is elliptical, FALSE if not |

Syntax (COM)

status
= DomeFeatureData-> get\_Elliptical( &Elliptical)

status
= DomeFeatureData-> put\_Elliptical( Elliptical)

|  |  |  |
| --- | --- | --- |
| Property: | (VARIANT\_BOOL) Elliptical | TRUE if the dome is elliptical, FALSE if not |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

This property does not affect geometry until you call Feature::ModifyDefinition.