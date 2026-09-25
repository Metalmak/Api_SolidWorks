<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__CreateDetailViewAt.htm -->

# DrawingDoc::CreateDetailViewAt

This
method is obsolete and has been superseded by [DrawingDoc::CreateDetailViewAt2](DrawingDoc__CreateDetailViewAt2.htm).

Description

This method creates a detail view at the specified location in sheet
space based on the selected closed contour.

Syntax (OLE Automation)

retval
= DrawingDoc.CreateDetailViewAt ( x, y, z )

| Input: | (double) x | x location |
| Input: | (double) y | y location |
| Input: | (double) z | z location |
| Return: | (BOOL) retval | TRUE if successfully created, FALSE if not |

Syntax (COM)

status = DrawingDoc->CreateDetailViewAt
( x, y, z, &retval )

| Input: | (double) x | x location |
| Input: | (double) y | y location |
| Input: | (double) z | z location |
| Output: | (VARIANT\_BOOL) retval | TRUE if successfully created, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks