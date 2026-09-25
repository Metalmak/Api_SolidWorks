<!-- source: obsoleteapi/Face/Face__GetEdgeCount.htm -->

# Face::GetEdgeCount

This
method is obsolete and has been superseded by Face2::GetEdgeCount.

Description

This method gets the count of the edges which bound this face.

Syntax (OLE Automation)

retval
= Face.GetEdgeCount ()

| Return: | (long) retval | Number of edges bounding this face |

Syntax (COM)

status = Face->GetEdgeCount ( &retval
)

| Output: | (long) retval | Number of edges bounding this face |
| Return: | (HRESULT) status | S\_OK if successful |