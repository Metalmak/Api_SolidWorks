<!-- source: obsoleteapi/Feature/Feature__IGetBody2.htm -->

# Feature::IGetBody2

This method is obsolete and has been superseded
by Feature::GetFaces
and Face2::GetBody.

Description

This method gets the body containing this feature.

Syntax (OLE Automation)

Not available.

Syntax (COM)

status = Feature->IGetBody2 ( &retval )

| Output: | (LPBODY2) retval | Pointer to the body |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This method returns a body
for a reference feature or an imported body; otherwise, NULL is returned.