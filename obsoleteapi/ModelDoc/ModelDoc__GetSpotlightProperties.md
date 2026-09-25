<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetSpotlightProperties.htm -->

# ModelDoc::GetSpotlightProperties

This
method is obsolete and has been superseded by ModelDoc2::GetSpotlightProperties.

Description

This method gets the spotlight properties.

Syntax (OLE Automation)

retval = ModelDoc.GetSpotlightProperties ( name,
&ambient, &diffuse, &specular, &color, &enabled, &fixed,
&x, &y, &z, &xTarget, &yTarget, &zTarget, &coneAngle
)

| Input: | (BSTR) name | Light name used internally by SolidWorks (returned by ModelDoc::GetLightSourceName) |
| Output: | (double) ambient | Light source ambient value |
| Output: | (double) diffuse | Light source diffuse value |
| Output: | (double) specular | Light source specular value |
| Output: | (long) color | COLORREF color value |
| Output: | (BOOL) enabled | TRUE if a light is enabled, FALSE if not |
| Output: | (BOOL) fixed | TRUE if a light is fixed, FALSE if not |
| Output: | (double) x | x location of the spot light |
| Output: | (double) y | y location of the spot light |
| Output: | (double) z | z location of the spot light |
| Output: | (double) xTarget | x location of the spot light target |
| Output: | (double) yTarget | y location of the spot light target |
| Output: | (double) zTarget | z location of the spot light target |
| Output: | (double) coneAngle | Cone angle through which the beam spreads in degrees |
| Return: | (BOOL) retval | TRUE if light properties determined without a problem, FALSE if not |

Syntax (COM)

status = ModelDoc->GetSpotlightProperties ( name,
&ambient, &diffuse, &specular, &color, &enabled, &fixed,
&x, &y, &z, &xTarget, &yTarget, &zTarget, &coneAngle,
&retval )

| Input: | (BSTR) name | Light name used internally by SolidWorks (returned by ModelDoc::GetLightSourceName) |
| Output: | (double) ambient | Light source ambient value |
| Output: | (double) diffuse | Light source diffuse value |
| Output: | (double) specular | Light source specular value |
| Output: | (long) color | COLORREF color value |
| Output: | (VARIANT\_BOOL) enabled | TRUE if a light is enabled, FALSE if not |
| Output: | (VARIANT\_BOOL) fixed | TRUE if a light is fixed, FALSE if not |
| Output: | (double) x | x location of the spot light |
| Output: | (double) y | y location of the spot light |
| Output: | (double) z | z location of the spot light |
| Output: | (double) xTarget | x location of the spot light target |
| Output: | (double) yTarget | y location of the spot light target |
| Output: | (double) zTarget | z location of the spot light target |
| Output: | (double) coneAngle | Cone angle through which the beam spreads in degrees |
| Output: | (VARIANT\_BOOL) retval | TRUE if light properties determined without a problem, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks