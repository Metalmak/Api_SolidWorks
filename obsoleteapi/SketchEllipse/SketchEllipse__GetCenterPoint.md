<!-- source: obsoleteapi/SketchEllipse/SketchEllipse__GetCenterPoint.htm -->

# SketchEllipse::GetCenterPoint

This method
is obsolete and has been superseded by SketchEllipse::GetCenterPoint2.

Description

This method gets the center point of this sketch
ellipse.

Syntax (OLE Automation)

retval = SketchEllipse.GetCenterPoint ( )

|  |  |  |
| --- | --- | --- |
| Return: | (VARIANT) retval | VARIANT of type docking state of the toolbar as defined in  swToolbarDockStatePosition\_e of 3 doubles (x,y,z), the ellipse center point |

Syntax (COM)status = SketchEllipse->IGetCenterPoint
( retval )

status = SketchEllipse->IGetCenterPoint2 ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (double\*) retval | Pointer to an array of 3 doubles (x,y,z), the ellipse center point |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks