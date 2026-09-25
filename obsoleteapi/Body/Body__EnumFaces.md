<!-- source: obsoleteapi/Body/Body__EnumFaces.htm -->

# Body::EnumFaces

This method is obsolete and has been superseded by Body2::EnumFaces.

Description

This method returns an enumerated list of the faces in a body.

Syntax (OLE Automation)

See Body::GetFirstFace and Face::GetNextFace.

Syntax (COM)

status
= Body->EnumFaces ( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (LPENUMFACES) retval | Enumerated list of faces |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks