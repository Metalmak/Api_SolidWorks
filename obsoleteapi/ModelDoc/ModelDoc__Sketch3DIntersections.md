<!-- source: obsoleteapi/ModelDoc/ModelDoc__Sketch3DIntersections.htm -->

# ModelDoc::Sketch3DIntersections

This method is obsolete
and has been superseded by ModelDoc2::Sketch3DIntersections.

Description

This methods creates new sketch segments based
on the selected surfaces. The new sketch segments are  added
either to the active sketch or to an appropriate new sketch.

Syntax (OLE Automation)

void ModelDoc.Sketch3DIntersections ( )

Syntax (COM)

status = ModelDoc->Sketch3DIntersections ( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successfu |

Remarks

If the active sketch is a 2D sketch and the intersection
curves are not in that plane, then the resulting sketch segments is projected
onto the plane of the sketch.