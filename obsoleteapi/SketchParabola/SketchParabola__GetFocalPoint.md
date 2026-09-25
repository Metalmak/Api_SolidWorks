<!-- source: obsoleteapi/SketchParabola/SketchParabola__GetFocalPoint.htm -->

# SketchParabola::GetFocalPoint

This
method is obsolete and has been superseded by SketchParabola::GetFocalPoint2.

Description

This method gets the focal point used to define
this sketch parabola.

Syntax (OLE Automation)

retval = SketchParabola.GetFocalPoint ( )

|  |  |  |
| --- | --- | --- |
| Return: | (VARIANT) retval | VARIANT of type SafeArray of 3 doubles (x,y,z), the parabola focal point |

Syntax (COM)

status = SketchParabola->IGetFocalPoint ( retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (double\*) retval | Pointer to an array of 3 doubles (x,y,z), the parabola focal point |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks