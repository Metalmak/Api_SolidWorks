<!-- source: obsoleteapi/Gtol/Gtol__GetUseDocTextFormat.htm -->

# Gtol::GetUseDocTextFormat

This method is obsolete and has been superseded
by Annotation::GetUseDocTextFormat.

Description

This
method gets whether or not this Gtol is currently using the document default
Gtol text format.

Syntax (OLE Automation)

retval
= Gtol.GetUseDocTextFormat ( )

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) retval | TRUE if the documents text formatting is used, FALSE if not |

Syntax (COM)

status = Gtol->GetUseDocTextFormat
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the documents text formatting is used, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |