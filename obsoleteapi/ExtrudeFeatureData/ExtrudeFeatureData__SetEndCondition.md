<!-- source: obsoleteapi/ExtrudeFeatureData/ExtrudeFeatureData__SetEndCondition.htm -->

# ExtrudeFeatureData::SetEndCondition

This
method is obsolete and has been superseded by ExtrudeFeatureData2::SetEndCondition.

Description

This method sets the end condition type of
the extrusion feature for forward or reverse direction.

Syntax (OLE Automation)

void ExtrudeFeatureData.SetEndCondition ( forward, endCondition )

|  |  |  |
| --- | --- | --- |
| Input: | (BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Input: | (int) endCondition | End condition type as defined in swEndConditions\_e |

Syntax (COM)

status = ExtrudeFeatureData->SetEndCondition (
forward, endCondition )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Input: | (int) endCondition | End condition type as defined in swEndConditions\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks