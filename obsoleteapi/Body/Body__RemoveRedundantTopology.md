<!-- source: obsoleteapi/Body/Body__RemoveRedundantTopology.htm -->

# Body::RemoveRedundantTopology

This method is obsolete and has been superseded by
Body2::RemoveRedundantTopology.

Description

This method removes redundant topology from the body.

Syntax (OLE Automation)

retval = Body.RemoveRedundantTopology
()

| Return: | (BOOL) retval | TRUE if the redundant topology was removed successfully, FALSE if it was not |

Syntax
(COM)

status = Body->RemoveRedundantTopology
( &retval )

| Output: | (VARIANT\_BOOL) retval | TRUE if the redundant topology was removed successfully, FALSE if it was not |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks