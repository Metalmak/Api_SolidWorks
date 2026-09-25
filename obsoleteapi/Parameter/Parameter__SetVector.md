<!-- source: obsoleteapi/Parameter/Parameter__SetVector.htm -->

# Parameter::SetVector

This method is obsolete and has been superseded by
Parameter::SetVector2.

Description

This method stores information of the type vector on a parameter.

Syntax (OLE Automation)

Not Available.

Syntax (COM)

status = Parameter->SetVector (
x, y, z, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (double) x | x vector value to be stored on the parameter |
| Input: | (double) y | y vector value to be stored on the parameter |
| Input: | (double) z | z vector value to be stored on the parameter |
| Output: | (VARIANT\_BOOL) retval | TRUE if successfully added, FALSE if not |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks