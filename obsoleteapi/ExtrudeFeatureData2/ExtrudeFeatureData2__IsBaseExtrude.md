<!-- source: obsoleteapi/ExtrudeFeatureData2/ExtrudeFeatureData2__IsBaseExtrude.htm -->

# ExtrudeFeatureData2::IsBaseExtrude

This method is obsolete and has been superseded
by Feature::IsBase2.

Description

This method gets whether the extrusion is a
base extrude feature.

Syntax (OLE Automation)

isBaseExtrude = ExtrudeFeatureData2.
IsBaseExtrude ( )

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) isBaseExtrude | TRUE if this extrusion is a base extrude feature, FALSE if not |

Syntax (COM)

status = ExtrudeFeatureData2-> IsBaseExtrude (
& isBaseExtrude)

| Output: | (VARIANT\_BOOL) isBaseExtrude | TRUE if this extrusion is a base extrude feature, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks