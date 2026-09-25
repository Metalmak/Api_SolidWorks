<!-- source: obsoleteapi/SketchEllipse/SketchEllipse__GetEndPoint.htm -->

# SketchEllipse::GetEndPoint

This method
is obsolete and has been superseded by SketchEllipse::GetEndPoint2.

Description

This method gets the end point of this sketch
ellipse.

Syntax (OLE Automation)

retval = SketchEllipse.GetEndPoint ( )

|  |  |  |
| --- | --- | --- |
| Return: | (VARIANT) retval | VARIANT of type SafeArray of 3 doubles (x,y,z), the ellipse end point |

Syntax (COM)

status = SketchEllipse->IGetEndPoint ( retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (double\*) retval | Pointer to an array of 3 doubles (x,y,z), the ellipse end point |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks