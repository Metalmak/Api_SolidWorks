<!-- source: obsoleteapi/DomeFeatureData/DomeFeatureData__ReleaseSelectionAccess.htm -->

# DomeFeatureData::ReleaseSelectionAccess

This method is obsolete and hs been superseded
by DomeFeatureData2::ReleaseSelectionAccess.

Description

This method releases access to selections used to define the dome feature.

Syntax (OLE Automation)

void DomeFeatureData.ReleaseSelectionAccess(
)

Syntax (COM)

status = DomeFeatureData->ReleaseSelectionAccess(
)

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This method restores the rollback state of the model after you call
DomeFeatureData::AccessSelections.