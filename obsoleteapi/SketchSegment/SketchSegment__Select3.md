<!-- source: obsoleteapi/SketchSegment/SketchSegment__Select3.htm -->

# SketchSegment::Select3

This method is obsolete and has been superseded
by SketchSegment::Select4.

Description

This method selects this sketch segment.

Syntax (OLE Automation)

retval = SketchSegment.Select3 ( Append, Mark, Callout
)

| Input: | (VARIANT\_BOOL) Append | TRUE appends the sketch segment to the selection list, FALSE replaces the current selection list with this sketch segment |
| Input: | (long) Mark | Value you want to use as a selection mark |
| Input: | (LPCALLOUT) Callout | Pointer to the associated callout |
| Output: | (VARIANT\_BOOL) retval | TRUE if the sketch segment was selected, FALSE if not |

Syntax (COM)

status = SketchSegment->Select3 ( Append, Mark,
Callout, &retval )

| Input: | (VARIANT\_BOOL) Append | TRUE appends the sketch segment to the selection list, FALSE replaces the current selection list with this sketch segment |
| Input: | (long) Mark | Value you want to use as a selection mark |
| Input: | (LPCALLOUT) Callout | Pointer to the associated callout |
| Output: | (VARIANT\_BOOL) retval | TRUE if the sketch segment was selected, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks