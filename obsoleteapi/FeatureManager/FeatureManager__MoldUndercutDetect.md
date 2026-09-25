<!-- source: obsoleteapi/FeatureManager/FeatureManager__MoldUndercutDetect.htm -->

# FeatureManager::MoldUndercutDetect

This method is obsolete and has been superseded
by FeatureManager::MoldUndercutDetect2.

Description

This method detects undercut
features.

Syntax (OLE Automation)

void = FeatureManager.MoldUndercutDetect ( colUndercut,
colBase, bCoordInput, dX, dY, dZ)

|  |  |  |
| --- | --- | --- |
| Input: | (long) colUndercut | Value (COLORREF type) that specifies the color for the faces that form an undercut |
| Input: | (long) colBase | Value (COLORREF type) that specifies the color for the faces that do not form undercuts, that is, all faces except the undercut faces |
| Input: | (VARIANT\_BOOL) bCoordInput | TRUE to enable coordinate input, FALSE to not |
| Input: | (double) dX | X coordinate |
| Input: | (double) dY | Y coordinate |
| Input: | (double) dZ | Z coordinate |

#

Syntax (COM)

status = FeatureManager->MoldUndercutDetect (
colUndercut, colBase, bCoordInput, dX, dY, dZ)

|  |  |  |
| --- | --- | --- |
| Input: | (long) colUndercut | Value (COLORREF type) that specifies the color for the faces that form an undercut |
| Input: | (long) colBase | Value (COLORREF type) that specifies the color for the faces that do not form undercuts, that is, all faces except the undercut faces |
| Input: | (VARIANT\_BOOL) bCoordInput | TRUE to enable coordinate input, FALSE to not |
| Input: | (double) dX | X coordinate |
| Input: | (double) dY | Y coordinate |
| Input: | (double) dZ | Z coordinate |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks