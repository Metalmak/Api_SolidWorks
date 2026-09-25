<!-- source: obsoleteapi/SketchSpline/SketchSpline__GetPointCount.htm -->

# SketchSpline::GetPointCount

This
method is obsolete and superseded by SketchSpline::IEnumPoints.

Description

This method determines the number of points
used when creating this sketch spline.

Syntax (OLE Automation)

retval = SketchSpline.GetPointCount ( )

|  |  |  |
| --- | --- | --- |
| Return: | (long) retval | Nnumber of points used in creating this spline |

Syntax (COM)

status = SketchSpline->GetPointCount ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (long) retval | Number of points used in creating this spline |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Use this value to allocate your memory for a call
to the COM version of  SketchSpline::GetPoints.