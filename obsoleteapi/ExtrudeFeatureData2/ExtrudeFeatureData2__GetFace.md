<!-- source: obsoleteapi/ExtrudeFeatureData2/ExtrudeFeatureData2__GetFace.htm -->

# ExtrudeFeatureData2::GetFace

This method is obsolete and has been superseded
by ExtrudeFeatureData2::GetEndConditionReference.

Description

This method gets the end condition face for
the extrusion feature in forward or reverse direction.

Syntax (OLE Automation)

face = ExtrudeFeatureData2.GetFace
( forward )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Return: | (LPDISPATCH) face | Dispatch pointer to the end condition face or NULL if the operation fails |

Syntax (COM)

status = ExtrudeFeatureData2->IGetFace ( forward,
&face )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) forward | TRUE for forward feature direction, FALSE for reverse |
| Output: | (LPFACE2) face | Pointer to the end condition face or NULL if the operation fails |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Use ExtrudeFeatureData2::AccessSelections before calling this method.