<!-- source: obsoleteapi/SketchContour/SketchContour__Select.htm -->

# SketchContour::Select

This method is obsolete and has been superseded
by SketchContour::Select2.

Description

This method selects and marks
this contour.

Syntax (OLE Automation)

retval = SketchContour.Select ( Append, Mark )

#

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) Append | TRUE appends the sketch contour to the current selection list, FALSE replaces the current selection list |
| Input: | (long) Mark | Value you want to use as a mark; this number is used by APIs that require ordered selection |
| Output: | (VARIANT\_BOOL) retval | TRUE if the contour is selected, FALSE if not |

#

Syntax (COM)

status = SketchContour->Select ( Append, Mark,
&retval )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) Append | TRUE appends the selected sketch contour to the current selection list, FALSE replaces the current selection list |
| Input: | (long) Mark | Value you want to use as a mark; this number is used by APIs that require ordered selection |
| Output: | (VARIANT\_BOOL) retval | TRUE if the contour is selected, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks