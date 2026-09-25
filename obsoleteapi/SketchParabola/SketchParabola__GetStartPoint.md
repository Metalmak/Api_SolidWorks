<!-- source: obsoleteapi/SketchParabola/SketchParabola__GetStartPoint.htm -->

# SketchParabola::GetStartPoint

This
method is obsolete and has been superseded by SketchParabola::GetStartPoint2.

Description

This method gets the start point of this sketch
parabola.

Syntax (OLE Automation)

retval = SketchParabola.GetStartPoint ( )

|  |  |  |
| --- | --- | --- |
| Return: | (VARIANT) retval | VARIANT of type SafeArray of 3 doubles (x,y,z), the parabola start point |

Syntax (COM)

status = SketchParabola->IGetStartPoint ( retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (double\*) retval | Pointer to an array of 3 doubles (x,y,z), the parabola start point |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks