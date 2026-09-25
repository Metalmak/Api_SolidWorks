<!-- source: obsoleteapi/Face/Face__RemoveRedundantTopology.htm -->

# Face::RemoveRedundantTopology

This
method is obsolete and has been superseded by Face2::RemoveRedundantTopology.

Description

This method removes redundant topology from the face.

Syntax (OLE Automation)

retval
= Face.RemoveRedundantTopology ()

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) retval | TRUE if the redundant topology was removed successfully, FALSE if it was not |

Syntax (COM)

status = Face->RemoveRedundantTopology
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the redundant topology was removed successfully, FALSE if it was not |
| Return: | (HRESULT)status | S\_OK if successful |