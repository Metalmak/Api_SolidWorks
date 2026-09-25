<!-- source: obsoleteapi/Body/Body__GetTessellation.htm -->

# Body::GetTessellation

This
method is obsolete and has been superseded by Body2::GetTessellation.

Description

This method gets the Tessellation object.

Syntax (OLE Automation)

retval = Body.GetTessellation ( FaceList )

| Input: | (VARIANT) FaceList | VARIANT of type SafeArray of pointers to dispatch objects, the array of faces to tessellate; if this is empty, then SolidWorks tessellates the body |
| Return: | (LPDISPATCH) retval | Pointer to the dispatch object for the Tessellation object |

Syntax (COM)

status = Body->IGetTessellation ( numOfFaces,
FaceList, &retval )

| Input: | (long) numOfFaces | Number of faces |
| Input: | (LPFACE\*) FaceList | Array of faces to tessellate of size numOfFaces; if this is NULL, then tessellate the body |
| Output: | (LPTESSELLATION) retval | Pointer to the Tessellation object |
| Return: | (HRESULT) status | S\_OK if successful. |

Remarks