<!-- source: obsoleteapi/Component/Component__GetTessTriStripEdges.htm -->

# Component::GetTessTriStripEdges

This
method is obsolete and has been superseded by Component2::GetTessTriStripEdges.

Description

This method gets the edge IDs for the triangle
strips.

Syntax (OLE Automation)

retval = Component.GetTessTriStripEdges ( VARIANT\* retval )

|  |  |  |
| --- | --- | --- |
| Input: | (double) x | X component of the direction vector |
| Input: | (double) y | Y component of the direction vector |
| Input: | (double) z | Z component of the direction vector |
| Input: | (BOOL) found | TRUE if a point was found |
| Input: | (VARIANT) startPoint | VARIANT of type SafeArray of 3 doubles (x,y,z) |
| Return: | (LPDISPATCH) retval | Pointer to a dispatch object, the newly created assembly or NULL if the operation fails |

Syntax (COM)

status = Component->GetTessTriStripEdges ( long\*
retval )

|  |  |  |
| --- | --- | --- |
| Input: | (double) x | X component of the direction vector |
| Input: | (double) y | Y component of the direction vector |
| Input: | (double) z | Z component of the direction vector |
| Input: | (VARIANT\_BOOL) found | TRUE if a point was found |
| Input: | (double\*) startPoint | Pointer to an array of 3 doubles (x,y,z) |
| Output: | (LPASSEMBLYDOC) retval | Pointer to a newly created assembly or NULL if the operation fails |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Tessellation information is
available only when the component is loaded as lightweight.