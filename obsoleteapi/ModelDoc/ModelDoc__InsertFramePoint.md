<!-- source: obsoleteapi/ModelDoc/ModelDoc__InsertFramePoint.htm -->

# ModelDoc::InsertFramePoint

This
method is obsolete and has been superseded by ModelDoc2::InsertFramePoint.

Description

This method inserts a frame point into the active
sketch for the selected spline at the given coordinates.

Syntax (OLE Automation)

void ModelDoc.InsertFramePoint ( x, y, z )

|  |  |  |
| --- | --- | --- |
| Input: | (double) x | x coordinate of frame point |
| Input: | (double) y | y coordinate of frame point |
| Input: | (double) z | z coordinate of frame point |

Syntax (COM)

status = ModelDoc->InsertFramePoint ( x, y, z
)

|  |  |  |
| --- | --- | --- |
| Input: | (double) x | x coordinate of frame point |
| Input: | (double) y | y coordinate of frame point |
| Input: | (double) z | z coordinate of frame point |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks