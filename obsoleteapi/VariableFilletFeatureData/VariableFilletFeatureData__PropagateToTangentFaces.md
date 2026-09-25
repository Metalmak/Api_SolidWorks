<!-- source: obsoleteapi/VariableFilletFeatureData/VariableFilletFeatureData__PropagateToTangentFaces.htm -->

# VariableFilletFeatureData::PropagateToTangentFaces

This
property is obsolete and has been superseded by VariableFilletFeatureData2::PropagateToTangentFaces.

Description

This property gets or sets whether to extend
fillet to all faces tangent to the selected face or edge.

Syntax (OLE Automation)

propTgtFaces = VariableFilletFeatureData.PropagateToTangentFaces  (VB
Get property)

VariableFilletFeatureData.PropagateToTangentFaces
= propTgtFaces  (VB Set property)

propTgtFaces = VariableFilletFeatureData.GetPropagateToTangentFaces
( ) (C++ Get property)

VariableFilletFeatureData.SetPropagateToTangentFaces
( propTgtFaces )  (C++ Set property)

| Property: | (BOOL) propTgtFaces | TRUE if variable fillet feature should extend fillet to all faces tangent to the selected face or edge, FALSE if not | The default fillet radius of the Simple Fillet feature. |

Syntax (COM)

status = VariableFilletFeatureData ->get\_PropagateToTangentFaces
( &propTgtFaces )

status = VariableFilletFeatureData ->put\_PropagateToTangentFaces
( propTgtFaces )

| Property: | (VARIANT\_BOOL) propTgtFaces | TRUE if variable fillet feature should extend fillet to all faces tangent to the selected face or edge, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks