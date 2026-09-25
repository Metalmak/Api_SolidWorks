<!-- source: obsoleteapi/SketchHatch/SketchHatch__Select3.htm -->

# SketchHatch::Select3

This method is obsolete and has been superseded
by SketchHatch::Select4.

Description

This method selects this sketch hatch.

Syntax (OLE Automation)

retval = SketchHatch.Select3 ( Append, Mark, Callout
)

| Input: | (BOOL) Append | TRUE appends the selections to the current selection list, FALSE replaces the current selection list |
| Input: | (long) Mark | Value you want to use as a mark; this number is used by API functions that require ordered selection |
| Input: | (LPCALLOUT) Callout | Pointer to the associated callout |
| Output: | (BOOL) retval | TRUE if item is successfully selected, FALSE if not |

Syntax (COM)

status = SketchHatch->Select3 ( Append, Mark,
Callout, &retval )

| Input: | (VARIANT\_BOOL) Append | TRUE appends the selections to the current selection list, FALSE replaces the current selection list |
| Input: | (long) Mark | Value you want to use as a mark; this number is used by API functions that require ordered selection |
| Input: | (LPCALLOUT) Callout | Pointer to the associated callout |
| Output: | (VARIANT\_BOOL) retval | TRUE if item is successfully selected, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks