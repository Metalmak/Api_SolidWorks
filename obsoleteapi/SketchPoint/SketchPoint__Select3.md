<!-- source: obsoleteapi/SketchPoint/SketchPoint__Select3.htm -->

# SketchPoint::Select3

This method is obsolete and has been superseded
by SketchPoint::Select4.

Description

This method selects this point.

Syntax (OLE Automation)

retval = SketchPoint.Select3 ( Append, Mark, Callout
)

|  |  |  |
| --- | --- | --- |
| Input: | (BOOL) Append | TRUE appends the sketch point to the selection list, FALSE replaces the current selection list with this sketch point |
| Input: | (long) Mark | Value you want to use as a selection mark |
| Input: | (LPCALLOUT) Callout | Pointer to the associated callout |
| Output: | (BOOL) retval | TRUE if the entity was selected, FALSE if not |

Syntax (COM)

status = SketchPoint->Select3 ( Append, Mark,
Callout, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) Append | TRUE appends the sketch point to the selection list, FALSE replaces the current selection list with this sketch point |
| Input: | (long) Mark | Value you want to use as a selection mark |
| Input: | (LPCALLOUT) Callout | Pointer to the associated callout |
| Output: | (VARIANT\_BOOL) retval | TRUE if the entity was selected, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks