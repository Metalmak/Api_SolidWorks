<!-- source: obsoleteapi/Face/Face__GetSurface.htm -->

# Face::GetSurface

This
method is obsolete and has been superseded byFace2::GetSurface.

Description

This method
finds the surface which is referenced by this face.

Syntax (OLE Automation)

retval
= Face.GetSurface ()

|  |  |  |
| --- | --- | --- |
| Return: | (LPDISPATCH) retval | Dispatch pointer to the underlying surface for this face |

Syntax (COM)

status = Face->IGetSurface ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (LPSURFACE) retval | Pointer to the underlying surface for this face |
| Return: | (HRESULT) status | S\_OK if successful |