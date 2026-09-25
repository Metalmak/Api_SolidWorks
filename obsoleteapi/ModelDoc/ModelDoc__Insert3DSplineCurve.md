<!-- source: obsoleteapi/ModelDoc/ModelDoc__Insert3DSplineCurve.htm -->

# ModelDoc::Insert3DSplineCurve

This
method is obsolete and has been superseded by ModelDoc2::Insert3DSplineCurve.

Description

This method inserts a 3D-spline curve through the selected reference
points.

Syntax (OLE Automation)

void ModelDoc.Insert3DSplineCurve (
curveClosed)

|  |  |  |
| --- | --- | --- |
| Input: | (BOOL) curveClosed | TRUE if you want the curve to be closed, FALSE otherwise |

Syntax (COM)

status = ModelDoc->Insert3DSplineCurve
( curveClosed )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) curveClosed | TRUE if you want the curve to be closed, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

To create 2D splines on a sketch, use ModelDoc::SketchSpline or ModelDoc::CreateSpline.