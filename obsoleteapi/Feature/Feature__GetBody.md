<!-- source: obsoleteapi/Feature/Feature__GetBody.htm -->

# Feature::GetBody

This
method is obsolete and has been superseded by Feature::GetFaces
and Face2::GetBody.

Description

For
a reference feature or imported body, this method gets the body containing
this feature.

Syntax (OLE Automation)

retval
= Feature.GetBody ( )

| Return: | (LPDISPATCH) retval | Dispatch pointer to the body |

Syntax (COM)

status = Feature->IGetBody ( &Body
)

| Output: | (LPBODY) Body | Pointer to the body |
| Return: | (HRESULT) status | S\_OK if successful |