<!-- source: obsoleteapi/Gtol/Gtol__SetTextFormat.htm -->

# Gtol::SetTextFormat

This method is obsolete and has been superseded
by Annotation::SetTextFormat.

Description

This
method sets the text format parameters.

Syntax (OLE Automation)

retval
= Gtol.SetTextFormat ( useDocFormat, textFormat )

|  |  |  |
| --- | --- | --- |
| Input: | (long) useDocFormat | Controls whether the Gtol uses the document text format or the textFormat argument values |
| Input: | (LPDISPATCH) textFormat | Formatting values |
| Return: | (BOOL) retval | TRUE if successfully set, FALSE if not |

Syntax (COM)

status
= Gtol->ISetTextFormat ( useDocFormat, textFormat, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long)useDocFormat | Controls whether the Gtol uses the document text format or the textFormat argument values |
| Input: | (LPTEXTFORMAT)textFormat | Formatting values |
| Output: | (VARIANT\_BOOL)retval | TRUE if successfully set, FALSE if not |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

This method sets the text formatting for this Gtol to the document text
formatting if useDocFormat is 1, or to the formatting specified in the
textFormat argument if useDocFormat is 0.