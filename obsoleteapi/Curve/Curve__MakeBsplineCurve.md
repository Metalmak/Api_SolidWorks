<!-- source: obsoleteapi/Curve/Curve__MakeBsplineCurve.htm -->

# Curve::MakeBsplineCurve

This method is obsolete and has been superseded
by Curve::MakeBsplineCurve2.

Description

This method creates a b-spline curve.

Syntax (OLE Automation)

retval = Curve.MakeBsplineCurve ( )

| Output: | (LPCURVE) retval | B-spline curve excluding lines and arcs |

Syntax (COM)

status = Curve->MakeBsplineCurve ( &retval
)

| Output: | (LPCURVE) retval | B-spline curve excluding lines and arcs |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This method uses the base
curve if it is a trimmed curve and excludes lines and arcs.