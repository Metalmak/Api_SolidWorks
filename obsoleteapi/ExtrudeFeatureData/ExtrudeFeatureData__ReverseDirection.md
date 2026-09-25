<!-- source: obsoleteapi/ExtrudeFeatureData/ExtrudeFeatureData__ReverseDirection.htm -->

# ExtrudeFeatureData::ReverseDirection

This
property is obsolete and has been superseded by ExtrudeFeatureData2::ReverseDirection.

Description

This property gets or sets whether to reverse
the direction of the extrusion feature.

Syntax (OLE Automation)

reverseDirection = ExtrudeFeatureData.ReverseDirection   (VB
Get property)

ExtrudeFeatureData.ReverseDirection = reverseDirection   (VB Set property)

reverseDirection = ExtrudeFeatureData.GetReverseDirection ( )  (C++
Get property)

ExtrudeFeatureData.SetReverseDirection (reverseDirection)  (C++ Set property)

| Property: | (BOOL) reverseDirection | TRUE reverses the direction of the extrusion feature, FALSE does not |

Syntax (COM)

status = ExtrudeFeatureData->get\_ReverseDirection
( &reverseDirection)

status = ExtrudeFeatureData->put\_ReverseDirection
(reverseDirection)

| Property: | (VARIANT\_BOOL) reverseDirection | TRUE reverses the direction of the extrusion feature, FALSE does not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks