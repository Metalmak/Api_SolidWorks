<!-- source: obsoleteapi/MateEntity/MateEntity__GetEntityType.htm -->

# MateEntity::GetEntityType

This method is obsolete and has been superseded
by MateEntity2::ReferenceType2.

Description

This method returns the entity type for this mate entity.

Syntax (OLE Automation)

retval = MateEntity.GetEntityType ()

|  |  |  |
| --- | --- | --- |
| Return: | (long) retval | Type of entity as defined in swMateEntityTypes\_e |

Syntax (COM)

status = MateEntity->GetEntityType
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (long) retval | Type of entity as defined in swMateEntityTypes\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Based on the entity type, you know what to expect in the Mate::GetMateParams
return value. To get to the MateEntity interface, use Mate::GetMateEntities.