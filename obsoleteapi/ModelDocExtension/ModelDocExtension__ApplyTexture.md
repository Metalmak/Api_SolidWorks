<!-- source: obsoleteapi/ModelDocExtension/ModelDocExtension__ApplyTexture.htm -->

# ModelDocExtension::ApplyTexture

This method is obsolete and has been superseded
by ModelDocExtension::SetTexture.

Description

This method applies texture
to all of the selected objects.

NOTE:
You cannot apply textures to drawing components.

Syntax (OLE Automation)

status = ModelDocExtension.ApplyTexture (Scale, angle,
textureFilename, blendColor)

|  |  |  |
| --- | --- | --- |
| Input: | (long) Scale | Scale factor (must be between 2 and 198) for texture |
| Input: | (double) angle | Angle in degrees (must be between 0° and 360°) at which to apply the texture |
| Input: | (BSTR) textureFilename | Path and filename of the texture to apply |
| Input: | (VARIANT\_BOOL) blendColor | TRUE to blend the current face color with the texture, FALSE to display the texture as is |
| Output: | (VARIANT\_BOOL) status | TRUE if texture applied, FALSE if not |

#

Syntax (COM)

status = ModelDocExtension->ApplyTexture ( Scale,
angle, textureFilename, blendColor, &status)

|  |  |  |
| --- | --- | --- |
| Input: | (long) Scale | Scale factor for texture; 1.0 fits the texture to the model |
| Input: | (double) angle | Angle in degrees at which to apply the texture |
| Input: | (BSTR) textureFilename | Path and filename of the texture to apply |
| Input: | (VARIANT\_BOOL) blendColor | TRUE to blend the current face color with the texture, FALSE to display the texture as is |
| Output: | (VARIANT\_BOOL) status | TRUE if texture applied, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks