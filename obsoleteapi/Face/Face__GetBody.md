<!-- source: obsoleteapi/Face/Face__GetBody.htm -->

# Face::GetBody

This
method is obsolete and has been superseded by Face2::GetBody.

Description

This method gets the body containing this face.

Syntax (OLE Automation)

retval
= Face.GetBody ()

|  |  |  |
| --- | --- | --- |
| Return: | (LPDISPATCH) retval | Dispatch pointer to the body |

Syntax (COM)

status = Face->IGetBody ( &Body
)

|  |  |  |
| --- | --- | --- |
| Output: | (LPBODY) Body | Pointer to the body |
| Return: | (HRESULT) status | S\_OK if successful |