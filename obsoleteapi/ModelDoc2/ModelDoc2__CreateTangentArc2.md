<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__CreateTangentArc2.htm -->

# ModelDoc2::CreateTangentArc2

This method is obsolete and has been superseded
by SketchManager::CreateTangentArc.

Description

This method creates a tangent arc.

Syntax (OLE Automation)

retval = ModelDoc2.CreateTangentArc2 ( p1x, p1y,
p1z, p2x, p2y, p2z, arcTypeIn )

#

| Input: | (double) p1x | x coordinate of start point in meters |
| Input: | (double) p1y | y coordinate of start point in meters |
| Input: | (double) p1z | z coordinate of start point in meters |
| Input: | (double) p2x | x coordinate of end point in meters |
| Input: | (double) p2y | y coordinate of end point in meters |
| Input: | (double) p2z | z coordinate of end point in meters |
| Input: | (long) arcTypeIn | Type of tangent arc as defined in swTangentArcTypes\_e |
| Output: | (VARIANT\_BOOL) retval | 1 = success, 0 = failure |

#

Syntax (COM)

status = ModelDoc2->CreateTangentArc2 ( p1x, p1y,
p1z, p2x, p2y, p2z, arcTypeIn, &retval )

| Input: | (double) p1x | x coordinate of start point in meters |
| Input: | (double) p1y | y coordinate of start point in meters |
| Input: | (double) p1z | z coordinate of start point in meters |
| Input: | (double) p2x | x coordinate of end point in meters |
| Input: | (double) p2y | y coordinate of end point in meters |
| Input: | (double) p2z | z coordinate of end point in meters |
| Input: | (long) arcTypeIn | Type of tangent arc as defined in swTangentArcTypes\_e |
| Output: | (VARIANT\_BOOL) retval | 1 = success, 0 = failure |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks