<!-- source: obsoleteapi/ModelDoc/ModelDoc__FontPoints.htm -->

# ModelDoc::FontPoints

This
method is obsolete and has been superseded by ModelDoc2::FontPoints.

Description

This method changes the height, in points, of the
font in the selected notes, dimensions, and Gtols.

Syntax (OLE Automation)

(void) ModelDoc.FontPoints
( points )

|  |  |  |
| --- | --- | --- |
| Input: | (short) points | Specifies the height, in points, of the font |

Syntax (COM)

status = ModelDoc->FontPoints
( points )

|  |  |  |
| --- | --- | --- |
| Input: | (short) points | Specifies the height, in points, of the font |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

You can also refer to the TextFormat object for
full control of text formatting. You can obtain this object by using the
GetTextFormat interfaces.