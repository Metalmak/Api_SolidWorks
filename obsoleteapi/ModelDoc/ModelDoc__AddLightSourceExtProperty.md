<!-- source: obsoleteapi/ModelDoc/ModelDoc__AddLightSourceExtProperty.htm -->

# ModelDoc::AddLightSourceExtProperty

This
method is obsolete and has been superseded by ModelDoc2::AddLightSourceExtProperty.

Description

This method stores a float, string, or integer value for light source.
This light source extension property is stored on the model document,
but is unique to the specified light source. To add the extension property,
you must first define the VARIANT type (float, string, or integer), give
your variable a value, and then call this method to place the value on
the light source for future reference.

Syntax (OLE Automation)

retval = ModelDoc.AddLightSourceExtProperty
( Id, PropertyExtension)

|  |  |  |
| --- | --- | --- |
| Input: | (long) Id | ID of the light source |
| Input: | (VARIANT) PropertyExtension | Value you wish to store for the light source |
| Return: | (long) retval | ID of the extension property |

Syntax (COM)

status = ModelDoc->AddLightSourceExtProperty
( Id, PropertyExtension, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long) Id | ID of the light source |
| Input: | (VARIANT) PropertyExtension | Value you wish to store for the light source |
| Output: | (long) retval | ID of the extension property |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks