<!-- source: obsoleteapi/VariableFilletFeatureData/VariableFilletFeatureData__OverflowType.htm -->

# VariableFilletFeatureData::OverflowType

This
property is obsolete and has been superseded by VariableFilletFeatureData2::OverflowType.

Description

This property gets or sets the variable fillet
feature overflow type.

Syntax (OLE Automation)

overflowType = VariableFilletFeatureData.OverflowType  (VB
Get property)

VariableFilletFeatureData.OverflowType = overflowType  (VB Set property)

overflowType = VariableFilletFeatureData.GetOverflowType (
) (C++ Get property)

VariableFilletFeatureData.SetOverflowType ( overflowType )  (C++ Set property)

| Property: | (int) overflowType | Overflow type of the variable fillet feature:   * 0 = Default * 1 = Keep edge * 2 = Keep surface |

Syntax (COM)

status = VariableFilletFeatureData ->get\_OverflowType
( &overflowType )

status = VariableFilletFeatureData ->put\_OverflowType
( overflowType )

| Property: | (int) overflowType | Overflow type of the variable fillet feature:   * 0 = Default * 1 = Keep edge * 2 = Keep surface |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks