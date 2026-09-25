<!-- source: obsoleteapi/Note/Note__GetUseDocTextFormat.htm -->

# Note::GetUseDocTextFormat

This method is obsolete and has been superseded
by Annotation::GetUseDocTextFormat.

Description

This method gets whether or
not the document default note text format is being used.

Syntax (OLE Automation)

retval = Note.GetUseDocTextFormat (
)

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) retval | TRUE if the documents text formatting is used, FALSE otherwise |

Syntax
(COM)

status = Note->GetUseDocTextFormat
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the documents text formatting is used, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks