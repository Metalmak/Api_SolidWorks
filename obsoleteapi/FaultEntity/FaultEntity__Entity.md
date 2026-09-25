<!-- source: obsoleteapi/FaultEntity/FaultEntity__Entity.htm -->

# FaultEntity::Entity

This property is obsolete and has been superseded
by FaultEntity::Entity2.

Description

This property gets the
entity.

Syntax (OLE Automation)

entity = FaultEntity.Entity ( index
) (VB Get property)

entity = FaultEntity.GetEntity ( index ) (C++ Get
property)

|  |  |  |
| --- | --- | --- |
| Input: | (long) index | 0-based index number indicating the entity to get |
| Output: | (LPENTITY) entity | Pointer to the Entity object |

#

Syntax (COM)

status = FaultEntity->get\_Entity
( index, &entity )

|  |  |  |
| --- | --- | --- |
| Input: | (long) index | 0-based index number indicating the entity to get |
| Output: | (LPENTITY) entity | Pointer to the Entity object |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks