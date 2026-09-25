<!-- source: obsoleteapi/Body2/Body2__Select.htm -->

# Body2::Select

This method is obsolete and has been superseded
by Body2::Select2.

Description

This method selects this body and marks it.

Syntax (OLE Automation)

retval = Body2.Select ( Append, Mark )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) Append | TRUE appends the selection list, FALSE replaces the selection list |
| Input: | (long) Mark | Value you want to use as a mark |
| Output: | (VARIANT\_BOOL) retval | TRUE if the feature was selected, FALSE if not |

Syntax (COM)

status = Body2->Select ( Append, Mark, &retval
)

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) Append | TRUE appends the selection list, FALSE replaces the selection list |
| Input: | (long) Mark | Value you want to use as a mark |
| Output: | (VARIANT\_BOOL) retval | TRUE if the feature was selected, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks