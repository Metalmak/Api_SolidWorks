<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__ReleaseSelectionAccess.htm -->

# WizardHoleFeatureData::ReleaseSelectionAccess

This method is obsolete and has been superseded
by WizardHoleFeatureData2::ReleaseSelectionAccess.

Description

This method releases access
to the selections used to define the hole wizard feature.

Syntax (OLE Automation)

void WizardHoleFeatureData.ReleaseSelectionAccess
( )

Syntax (COM)

status = WizardHoleFeatureData ->ReleaseSelectionAccess
( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

WizardHoleFeatureData::AccessSelections puts the
model into a rollback state to allow access to the selections that define
the hole wizard feature. You must use WizardHoleFeatureData::ReleaseSelectionAccess
to restore the rollback state unless you call Feature::ModifyDefinition.