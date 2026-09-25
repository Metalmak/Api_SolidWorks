<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetAmbientLightProperties.htm -->

# ModelDoc::GetAmbientLightProperties

This
method is obsolete and has been superseded by ModelDoc2::GetAmbientLightProperties.

Description

This method gets the ambient light properties.

Syntax (OLE Automation)

retval = ModelDoc.GetAmbientLightProperties ( name,
&ambient, &diffuse, &specular, &color, &enabled, &fixed
)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) name | Light name |
| Output: | (double) ambient | Light source ambient value |
| Output: | (double) diffuse | Light source diffuse value |
| Output: | (double) specular | Light source specular value |
| Output: | (long) color | COLORREF color value |
| Output: | (BOOL) enabled | TRUE if a light is enabled, FALSE if not |
| Output: | (BOOL) fixed | TRUE if a light is fixed, FALSE if not |
| Return: | (BOOL) retval | TRUE if light properties determined without a problem, FALSE if not |

Syntax (COM)

status = ModelDoc->GetAmbientLightProperties (name,
&ambient, &diffuse, &specular, &color, &enabled, &fixed,
&retval )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) name | Light name |
| Output: | (double) ambient | Light source ambient value |
| Output: | (double) diffuse | Light source diffuse value |
| Output: | (double) specular | Light source specular value |
| Output: | (long) color | COLORREF color value |
| Output: | (VARIANT\_BOOL) enabled | TRUE if a light is enabled, FALSE if not |
| Output: | (VARIANT\_BOOL) fixed | TRUE if a light is fixed, FALSE if not |
| Output: | (VARIANT\_BOOL) retval | TRUE if light properties determined without a problem, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks