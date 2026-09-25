<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__InsertCenterMark.htm -->

# DrawingDoc::InsertCenterMark

This method is obsolete and has been superseded
by DrawingDoc::InsertCenterMark2.

Description

This method creates a center mark from the
last edge selection.

Syntax (OLE Automation)

retval = DrawingDoc.InsertCenterMark ( UseDoc, Size,
ShowLines, Angle )

| Input: | (BOOL) UseDoc | TRUE uses the document defaults for center mark display attributes, FALSE uses the values specified in the Size and ShowLines arguments |
| Input: | (double) Size | Center mark size in meters; half the size of the plus sign (+) at the circle center |
| Input: | (BOOL) ShowLines | TRUE displays the center mark lines, FALSE displays only the plus sign (+) at the circle center |
| Input: | (double) Angle | Angle that the center mark is rotated in radians |
| Return: | (LPDISPATCH) retval | Dispatch pointer to the new center mark |

Syntax (COM)

status = DrawingDoc->InsertCenterMark ( UseDoc,
Size, ShowLines, Angle, &retval )

| Input: | (VARIANT\_BOOL) UseDoc | TRUE uses the document defaults for center mark display attributes, FALSE uses the values specified in the Size and ShowLines arguments |
| Input: | (double) Size | Center mark size in meters; half the size of the plus sign (+)  at the circle center |
| Input: | (VARIANT\_BOOL) ShowLines | TRUE displays the center mark lines, FALSE displays only the plus sign (+) at the circle center |
| Input: | (double) Angle | Angle that the center mark is rotated in radians |
| Output: | (LPCENTERMARK) retval | Pointer to the new center mark |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

In addition to Size being half the size of the
plus sign (+) at the circle center, it is also the distance that the center
mark lines overshoot the circle if ShowLines is TRUE.