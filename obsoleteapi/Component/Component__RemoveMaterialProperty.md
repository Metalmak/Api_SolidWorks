<!-- source: obsoleteapi/Component/Component__RemoveMaterialProperty.htm -->

# Component::RemoveMaterialProperty

This
property is obsolete and has been superseded by [Component2::RemoveMaterialProperty](../Component2/Component2__RemoveMaterialProperty.htm).

Description

This method removes material property values
from the component.

Syntax (OLE Automation)

retval = Component.RemoveMaterialProperty ( )

| Return: | (BOOL) retval | TRUE if the material property was removed, FALSE if not |

Syntax (COM)

status = Component->RemoveMaterialProperty ( &retval
)

| Output: | (VARIANT\_BOOL) retval | TRUE if the material property was removed, FALSE if not |
| Return: | (HRESULT) retval | S\_OK if successful; S\_FALSE otherwise |

Remarks

This method is intended to be used on components
whose material property value has changed (for example, color).