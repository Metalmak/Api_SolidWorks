<!-- source: obsoleteapi/Body/Body_GetType.htm -->

# Body::GetType

This method is obsolete and has been superseded
by Body2::GetType.

Description

This method gets the body type.

Syntax (OLE Automation)

retval = Body.GetType ( )

|  |  |  |
| --- | --- | --- |
| Return: | (long) retval | Body type as defined in swBodyType\_e |

Syntax (COM)

status = Body->GetType ( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (long) retval | Body type as defined in swBodyType\_e |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

Empty is a special case that SolidWorks returns
if the interface pointer or underlying body pointer is NULL, indicating
the body is non-existent.