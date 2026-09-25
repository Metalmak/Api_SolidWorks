<!-- source: obsoleteapi/Parameter/Parameter__SetStringValue.htm -->

# Parameter::SetStringValue

This method is obsolete and has been superseded by
Parameter::SetStringValue2.

Description

This method adds string data to a parameter.

Syntax (OLE Automation)

retval = Parameter.SetStringValue (
StringValue)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) StringValue | Value for the parameter |
| Return: | (BOOL) retval | TRUE if successfully added, FALSE if not |

Syntax (COM)

status = Parameter->SetStringValue
( StringValue, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) StringValue | Value for the parameter |
| Output: | (VARIANT\_BOOL) retval | TRUE if successfully added, if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks