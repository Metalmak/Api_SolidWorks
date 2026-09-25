<!-- source: obsoleteapi/ExtrudeFeatureData/ExtrudeFeatureData__CapEnds.htm -->

# ExtrudeFeatureData::CapEnds

This
property is obsolete and has been superseded by ExtrudeFeatureData2::CapEnds.

Description

This property gets or sets whether the ends
of this thin base extrude feature are capped.

Syntax (OLE Automation)

capEnds = ExtrudeFeatureData.CapEnds (VB Get property)

ExtrudeFeatureData.CapEnds = capEnds (VB Set property)

capEnds = ExtrudeFeatureData.GetCapEnds ( ) (C++
Get property)

ExtrudeFeatureData.SetCapEnds ( capEnds ) (C++ Set
property)

|  |  |  |
| --- | --- | --- |
| Property: | (VARIANT\_BOOL) capEnds | TRUE caps the ends, FALSE does not |

Syntax (COM)

status = ExtrudeFeatureData->get\_CapEnds ( &capEnds
)

status = ExtrudeFeatureData->put\_CapEnds ( capEnds
)

|  |  |  |
| --- | --- | --- |
| Property: | (VARIANT\_BOOL) capEnds | TRUE caps the ends, FALSE does not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks