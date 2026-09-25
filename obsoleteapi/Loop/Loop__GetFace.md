<!-- source: obsoleteapi/Loop/Loop__GetFace.htm -->

# Loop::GetFace

This method is obsolete
and has been superseded by Loop2::GetFace.

Description

This method gets the face containing this loop

Syntax (OLE Automation)

retval = Loop.GetFace ()

|  |  |  |
| --- | --- | --- |
| Return: | (LPDISPATCH) retval | Pointer to a Dispatch object, the face |

Syntax (COM)

status = Loop->IGetFace ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (LPFACE) retval | Pointer to the face |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks