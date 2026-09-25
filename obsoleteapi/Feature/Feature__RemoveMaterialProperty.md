<!-- source: obsoleteapi/Feature/Feature__RemoveMaterialProperty.htm -->

# Feature::RemoveMaterialProperty

This method is obsolete and has been superseded
by Feature::RemoveMaterialProperty2.

Description

This method removes material property values
from this feature.

Syntax (OLE Automation)

retval = Feature.RemoveMaterialProperty ( )

| Return: | (VARIANT\_BOOL) retval | TRUE if the material property value has been removed from the feature, FALSE if not |

Syntax (COM)

status = Feature->RemoveMaterialProperty ( &retval
)

| Output: | (VARIANT\_BOOL) retval | TRUE if the material property value has been removed from the feature, FALSE if not |
| Return: | (HRESULT) retval | S\_OK if successful |

Remarks

This method is intended to be used on features
that have a changed material property value (for example, color).