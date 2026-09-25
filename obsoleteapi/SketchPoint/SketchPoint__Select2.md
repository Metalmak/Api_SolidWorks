<!-- source: obsoleteapi/SketchPoint/SketchPoint__Select2.htm -->

# SketchPoint::Select2

This method is obsolete and has been superseded
by [SketchPoint::Select3](SketchPoint__Select3.htm).

Description

This method selects this point and marks it.

Syntax (OLE Automation)

retval = SketchPoint.Select2 ( Append, Mark )

#

| Input: | (VARIANT\_BOOL) Append | TRUE appends the selections to the current selection list, FALSE replaces the current selection list with this item |
| Input: | (long) Mark | Value you want to use as a mark; this number is used by certain API functions that require ordered selection |
| Output: | (VARIANT\_BOOL) retval | TRUE if the sketch point was selected, FALSE if not |

#

Syntax (COM)

status = SketchPoint->Select2 ( Append, Mark,
&retval )

| Input: | (VARIANT\_BOOL) Append | TRUE appends the selections to the current selection list, FALSE replaces the current selection list with this item |
| Input: | (long) Mark | Value you want to use as a mark; this number is used by API functions that require ordered selection |
| Output: | (VARIANT\_BOOL) retval | TRUE if the sketch point was selected, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks