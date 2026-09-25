<!-- source: obsoleteapi/VariableFilletFeatureData/VariableFilletFeatureData__SetRadius.htm -->

# VariableFilletFeatureData::SetRadius

This
method is obsolete and has been superseded by VariableFilletFeatureData2::SetRadius.

Description

This method sets the radius value for specified
fillet item.

Syntax (OLE Automation)

void VariableFilletFeatureData.SetRadius ( pVertex,
radius )

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pVertex | Vertex at which the radius value is desired |
| Input: | (double) radius | Radius value |

Syntax (COM)

status = VariableFilletFeatureData->ISetRadius
( pVertex, radius )

|  |  |  |
| --- | --- | --- |
| Input: | (LPVERTEX) pVertex | Vertex at which the radius value is desired |
| Input: | (double) radius | Radius value |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks