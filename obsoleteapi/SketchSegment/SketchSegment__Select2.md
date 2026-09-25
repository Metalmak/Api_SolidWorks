<!-- source: obsoleteapi/SketchSegment/SketchSegment__Select2.htm -->

# SketchSegment::Select2

This method is obsolete and has been superseded
by [SketchSegment::Select3](SketchSegment__Select3.htm).

Description

This method selects this segment and marks
it.

Syntax (OLE Automation)

retval = SketchSegment.Select2 ( Append, Mark )

#

| Input: | (VARIANT\_BOOL) Append | TRUE appends the selections to the current selection list, FALSE replaces the current selection list with this sketch segment |
| Input: | (long) Mark | Value you want to use as a mark; this number is used by certain API functions that require ordered selection |
| Output: | (VARIANT\_BOOL) retval | TRUE if the feature was selected, FALSE if not |

#

Syntax (COM)

status = SketchSegment->Select2 ( Append, Mark,
&retval )

| Input: | (VARIANT\_BOOL) Append | TRUE appends the selections to the current selection list, FALSE replaces the current selection list with this sketch segment |
| Input: | (long) Mark | Value you want to use as a mark; this number is used by certain API functions that require ordered selection |
| Output: | (VARIANT\_BOOL) retval | TRUE if the sketch segment was selected, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks