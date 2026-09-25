<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__SimplifySpline.htm -->

# ModelDoc2::SimplifySpline

This method is obsolete and has been superseded
by SketchSpline::Simplify.

Description

This method simplifies a spline in the current
model document.

NOTE:
The sketch must be in editing mode and a spline must be preselected.

Syntax (OLE Automation)

ModelDoc2.SimplifySpline ( toleranceIn )

#

|  |  |  |
| --- | --- | --- |
| Input: | (double) toleranceIn | Smoothing factor, in meters, to use to simplify sketch |

#

Syntax (COM)

status = ModelDoc2->SimplifySpline ( toleranceIn
)

|  |  |  |
| --- | --- | --- |
| Input: | (double) toleranceIn | Smoothing factor,in meters, to use to simplify sketch |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks