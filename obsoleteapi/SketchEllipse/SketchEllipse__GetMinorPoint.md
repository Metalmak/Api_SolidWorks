<!-- source: obsoleteapi/SketchEllipse/SketchEllipse__GetMinorPoint.htm -->

# SketchEllipse::GetMinorPoint

This method
is obsolete and has been superseded by SketchEllipse::GetMinorPoint2.

Description

This method gets the minor point used to define
this sketch ellipse.

Syntax (OLE Automation)

retval = SketchEllipse.GetMinorPoint ( )

|  |  |  |
| --- | --- | --- |
| Return: | (VARIANT) retval | VARIANT of type SafeArray of 3 doubles (x,y,z), the ellipse minor sketch point |

Syntax (COM)

status = SketchEllipse->IGetMinorPoint ( retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (double\*) retval | Pointer to an array of 3 doubles (x,y,z), the ellipse minor sketch point |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks