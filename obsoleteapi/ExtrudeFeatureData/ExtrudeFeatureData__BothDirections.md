<!-- source: obsoleteapi/ExtrudeFeatureData/ExtrudeFeatureData__BothDirections.htm -->

# ExtrudeFeatureData::BothDirections

This
property is obsolete and has been superseded by ExtrudeFeatureData2::BothDirections.

Description

This property gets or sets whether the extrusion
is in both directions.

Syntax (OLE Automation)

bothDirections = ExtrudeFeatureData.BothDirections  (VB
Get property)

ExtrudeFeatureData.BothDirections = bothDirections  (VB Set property)

bothDirections = ExtrudeFeatureData.GetBothDirections ( )  (C++
Get property)

ExtrudeFeatureData.SetBothDirections (bothDirections)  (C++ Set property)

| Property: | (BOOL) bothDirections | TRUE if extrusion is in both directions, FALSE if not |

Syntax (COM)

status = ExtrudeFeatureData->get\_BothDirections
( & bothDirections )

status = ExtrudeFeatureData->put\_BothDirections
( bothDirections )

| Property: | (VARIANT\_BOOL) bothDirections | TRUE if extrusion is in both directions, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks