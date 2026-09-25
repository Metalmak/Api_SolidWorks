<!-- source: obsoleteapi/Body/Body__GetProcessedBodyWithSelFace.htm -->

# Body::GetProcessedBodyWithSelFace

This
method is obsolete and has been superseded by Body2::GetProcessedBodyWithSelFace.

Description

This method returns a pointer or dispatch pointer to a processed body.

Syntax (OLE Automation)

retval
= Body.GetProcessedBodyWithSelFace ( )

| Return: | (LPDISPATCH) retval | Dispatch object for the body; this body is a copy of the body for this part |

Syntax (COM)

status
= Body->IGetProcessedBodyWithSelFace ( &retval )

| Output: | (LPBODY)retval | Pointer to the body; this body is a copy of the body for this part |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks