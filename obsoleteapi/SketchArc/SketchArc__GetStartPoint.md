<!-- source: obsoleteapi/SketchArc/SketchArc__GetStartPoint.htm -->

# SketchArc::GetStartPoint

This method is obsolete and has been superseded by
SketchArc::GetStartPoint2.

Description

This method gets the startpoint of this sketch
arc.

Syntax (OLE Automation)

retval = SketchArc.GetStartPoint ( )

| Return: | (VARIANT) retval | VARIANT of type SafeArray of 3 doubles (x,y,z), the arc startpoint |

Syntax (COM)

status = SketchArc->IGetStartPoint ( retval )

| Output: | (double\*) retval | pointer to an array of 3 doubles (x,y,z), the arc startpoint |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks