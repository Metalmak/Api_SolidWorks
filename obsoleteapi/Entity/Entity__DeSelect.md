<!-- source: obsoleteapi/Entity/Entity__DeSelect.htm -->

# Entity::DeSelect

This
method is obsolete and has been superseded by ModelDoc2::DeSelectByID.

Description

This method deselects this entity.

Syntax (OLE Automation)

retval = Entity.DeSelect ( )

| Return: | (BOOL) retval | TRUE if the entity was deselected, FALSE if not |

Syntax (COM)

status = Entity->DeSelect ( &retval )

| Output: | (VARIANT\_BOOL) retval | TRUE if the entity was deselected, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Use ModelDoc2::DeSelectByID instead of using this
method. This method does not work well when a PropertyManager page is
open or a command is running. ModelDoc2::DeSelectByID handles selection
correctly whether or not a command is running.