<!-- source: obsoleteapi/ExtrudeFeatureData/ExtrudeFeatureData__ReleaseSelectionAccess.htm -->

# ExtrudeFeatureData::ReleaseSelectionAccess

This
method is obsolete and has been superseded by ExtrudeFeatureData2::ReleaseSelectionAccess.

Description

This method releases access to the selections
used to define the extrude feature.

Syntax (OLE Automation)

void ExtrudeFeatureData.ReleaseSelectionAccess (
)

Syntax (COM)

status = ExtrudeFeatureData->ReleaseSelectionAccess
( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

ExtrudeFeatureData2::AccessSelections puts the
model into a rollback state to allow access to the selections that define
the extrusion feature. Use ReleaseSelectionAccess to restore the rollback
state, unless you call Feature::ModifyDefinition.