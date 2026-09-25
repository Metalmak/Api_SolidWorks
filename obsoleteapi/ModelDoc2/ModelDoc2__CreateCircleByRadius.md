<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__CreateCircleByRadius.htm -->

# ModelDoc2::CreateCircleByRadius

This
method is obsolete and has been superseded by [ModelDoc2::CreateCircleByRadius2](ModelDoc2__CreateCircleByRadius2.htm).

Description

This method creates a circle with P1 as the centerpoint and with radius
as the radius.

Syntax (OLE Automation)

retval = ModelDoc2.CreateCircleByRadius
( P1, radius)

| Input: | (VARIANT) P1 | VARIANT of type SafeArray of 3 doubles (x1,y1, z1) in meters that describe the center point of the arc |
| Input: | (double) radius | Radius of circle in meters |
| Return: | (VARIANT\_BOOL) retval | TRUE if success, FALSE if fail |

Syntax (COM)

status = ModelDoc2->ICreateCircleByRadius
( P1, radius )

|  |  |  |
| --- | --- | --- |
| Input: | (double\*) P1 | Pointer to an array of 3 doubles (x1,y1, z1) in meters that describe the center point of the arc. |
| Input: | (double) radius | Radius of circle in meters |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks