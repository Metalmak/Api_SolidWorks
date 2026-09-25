<!-- source: obsoleteapi/PartDoc/PartDoc__FeatureRevolveCut.htm -->

# PartDoc::FeatureRevolveCut

This method is obsolete and has been superseded
by FeatureManager::FeatureRevolveCut.

Description

This method creates a revolved feature cut.

Syntax (OLE Automation)

void PartDoc.FeatureRevolveCut ( angle,
reverseDir, angle2, revType)

|  |  |  |
| --- | --- | --- |
| Input: | (double) angle | Angle of revolution in radians |
| Input: | (VARIANT\_BOOL) reverseDir | Positive or negative angle (TRUE or FALSE) |
| Input: | (double) angle2 | Angle of revolution in radians |
| Input: | (long) revType | Type of revolution |

Syntax (COM)

status = PartDoc->FeatureRevolveCut
( angle, reverseDir, angle2, revType )

|  |  |  |
| --- | --- | --- |
| Input: | (double) angle | Angle of revolution in radians |
| Input: | (VARIANT\_BOOL) reverseDir | Positive or negative angle (TRUE or FALSE) |
| Input: | (double) angle2 | Angle of revolution in radians |
| Input: | (long) revType | Type of revolution |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks