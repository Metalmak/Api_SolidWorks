<!-- source: obsoleteapi/SketchArc/SketchArc__GetCenterPoint.htm -->

# SketchArc::GetCenterPoint

This method
is obsolete and has been superseded by SketchArc::GetCenterPoint2.

Description

This method gets the centerpoint of this sketch
arc.

Syntax (OLE Automation)

retval = SketchArc.GetCenterPoint ( )

|  |  |  |
| --- | --- | --- |
| Return: | (VARIANT) retval | VARIANT of type SafeArray of 3 doubles (x,y,z), the arc centerpoint |

Syntax (COM)

status = SketchArc->IGetCenterPoint ( retval )

|  |  |  |
| --- | --- | --- |
| Output: | (double\*) retval | pointer to an array of 3 doubles (x,y,z), the arc centerpoint |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks