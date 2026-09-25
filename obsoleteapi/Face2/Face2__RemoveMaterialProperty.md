<!-- source: obsoleteapi/Face2/Face2__RemoveMaterialProperty.htm -->

# Face2::RemoveMaterialProperty

This method is obsolete and is superseded
by Face2::RemoveMaterialProperty2.

Description

This method removes the material property values
from this face.

Syntax (OLE Automation)

retval = Face2.RemoveMaterialProperty ( )

| Return: | (BOOL) retval | TRUE if the material property has been removed, FALSE if not |

Syntax (COM)

status = Face2->RemoveMaterialProperty ( &retval
)

| Output: | (VARIANT\_BOOL) retval | TRUE if the material property has been removed, FALSE if not |
| Return: | (HRESULT) retval | S\_OK if successful |

Remarks

This method is intended to be used on faces with
changed material properties (for example, color).