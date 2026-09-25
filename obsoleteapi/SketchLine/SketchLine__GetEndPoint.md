<!-- source: obsoleteapi/SketchLine/SketchLine__GetEndPoint.htm -->

# SketchLine::GetEndPoint

This method
is obsolete and has been superseded by SketchLine::GetEndPoint2.

Description

This method gets the endpoint of this sketch
line.

Syntax (OLE Automation)

retval = SketchLine.GetEndPoint ( )

| Return: | (VARIANT) retval | VARIANT of type SafeArray of 3 doubles (x,y,z), the line endpoint |

Syntax (COM)

status = SketchLine->IGetEndPoint ( retval )

|  |  |  |
| --- | --- | --- |
| Output: | (double\*) retval | pointer to an array of 3 doubles (x,y,z), the line endpoint |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks