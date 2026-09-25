<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__CreateSectionViewAt.htm -->

# DrawingDoc::CreateSectionViewAt

This
method is obsolete and has been superseded by [DrawingDoc::CreateSectionViewAt2](DrawingDoc__CreateSectionViewAt2.htm).

Description

This method creates a new section view at the specified location on
the drawing.

Syntax (OLE Automation)

retval
= DrawingDoc.CreateSectionViewAt ( x, y, z, notAligned, isOffsetSection
)

| Input: | (double) x | X position on the drawing sheet for the center of the drawing view |
| Input: | (double) y | Y position on the drawing sheet for the center of the drawing view |
| Input: | (double) z | Z position on the drawing sheet for the center of the drawing view |
| Input: | (BOOL) notAligned | TRUE breaks the alignment from the parent view, FALSE snaps into alignment with the parent view |
| Input: | (BOOL) isOffsetSection | TRUE creates an aligned section (two lines at an angle), FALSE creates a normal projection section view |
| Return: | (BOOL) retval | TRUE if successful |

Syntax (COM)

status = DrawingDoc->CreateSectionViewAt
( x, y, z, notAligned, isOffsetSection, &retval )

| Input: | (double) x | X position on the drawing sheet for the center of the drawing view |
| Input: | (double) y | Y position on the drawing sheet for the center of the drawing view |
| Input: | (double) z | Z position on the drawing sheet for the center of the drawing view |
| Input: | (VARIANT\_BOOL) notAligned | TRUE breaks the alignment from the parent view, FALSE snaps into alignment with the parent view |
| Input: | (VARIANT\_BOOL) isOffsetSection | TRUE creates an aligned section (two lines at an angle), FALSE creates a normal projection section view |
| Output: | (VARIANT\_BOOL) retval | TRUE if successful |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks