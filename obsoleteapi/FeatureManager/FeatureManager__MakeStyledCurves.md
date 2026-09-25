<!-- source: obsoleteapi/FeatureManager/FeatureManager__MakeStyledCurves.htm -->

# FeatureManager::MakeStyledCurves

This method is obsolete and has been superseded
by FeatureManager::MakeStyledCurves2.

Description

This method fits a spline to sketch segments
to make a smooth edge on the model.

Syntax (OLE Automation)

void = FeatureManager.MakeStyledCurves ( tol, mode
)

#

|  |  |  |
| --- | --- | --- |
| Input: | (double) tol | Deviation permitted from the selected geometry |
| Input: | (long) mode | * 1   = Convert the selected geometry to construction geometry * 11   = delete the selected geometry |

#

Syntax (COM)

status = FeatureManager->MakeStyledCurves ( tol,
mode )

|  |  |  |
| --- | --- | --- |
| Input: | (double) tol | Deviation permitted from the selected geometry |
| Input: | (long) mode | * 1   = Convert the selected geometry to construction geometry * 11   = delete the selected geometry |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks

All of the selected sketch
segments must be connected or this method will fail.