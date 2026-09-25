<!-- source: obsoleteapi/ModelDoc/ModelDoc__SetDirectionLightProperties.htm -->

# ModelDoc::SetDirectionLightProperties

This
method is obsolete and has been superseded by ModelDoc2::SetDirectionLightProperties.

Description

This method sets direction light properties.

Syntax (OLE Automation)

retval = ModelDoc.SetDirectionLightProperties ( name,
ambient, diffuse, specular, color, enabled, fixed, xDir, yDir, zDir )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR)name | Light name to modify |
| Input: | (double)ambient | Light source ambient value |
| Input: | (double)diffuse | Light source diffuse value |
| Input: | (double)specular | Light source specular value |
| Input: | (long)color | COLORREF color value |
| Input: | (BOOL)enabled | TRUE if the light should be enabled |
| Input: | (BOOL)fixed | TRUE if the light should be fixed |
| Input: | (double)xDir | x component of the light direction vector |
| Input: | (double)yDir | y component of the light direction vector |
| Input: | (double)zDir | z component of the light direction vector |
| Return: | (BOOL) retval | TRUE if light properties were changed successfully |

Syntax (COM)

status = ModelDoc->SetDirectionLightProperties
(name, ambient, diffuse, specular, color, enabled, fixed, xDir, yDir,
zDir, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR)name | Light name to be modified |
| Input: | (double)ambient | Light source ambient value |
| Input: | (double)diffuse | Light source diffuse value |
| Input: | (double)specular | Light source specular value |
| Input: | (long)color | COLORREF color value |
| Input: | (VARIANT\_BOOL)enabled | TRUE if the light should be enabled |
| Input: | (VARIANT\_BOOL)fixed | TRUE if the light should be fixed |
| Input: | (double)xDir | x component of the light direction vector |
| Input: | (double)yDir | y component of the light direction vector |
| Input: | (double)zDir | z component of the light direction vector |
| Output: | (VARIANT\_BOOL) retval | TRUE if light properties were changed successfully |
| Return: | (HRESULT) status | S\_OK if successful; S\_FALSE otherwise |

Remarks