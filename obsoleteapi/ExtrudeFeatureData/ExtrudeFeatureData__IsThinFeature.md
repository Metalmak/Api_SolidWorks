<!-- source: obsoleteapi/ExtrudeFeatureData/ExtrudeFeatureData__IsThinFeature.htm -->

# ExtrudeFeatureData::IsThinFeature

This
method is obsolete and has been superseded by ExtrudeFeatureData2::IsThinFeature.

Description

This method gets whether the extrusion is a
thin feature.

Syntax (OLE Automation)

isThinFeature = ExtrudeFeatureData.IsThinFeature
( )

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) isThinFeature | TRUE if extrusion is a thin feature, FALSE if not |

Syntax (COM)

status = ExtrudeFeatureData->get\_IsThinFeature
( &isThinFeature )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) isThinFeature | TRUE if extrusion is a thin feature, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks