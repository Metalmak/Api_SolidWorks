<!-- source: obsoleteapi/RevolveFeatureData/RevolveFeatureData__Type.htm -->

# RevolveFeatureData::Type

This
property is obsolete and has been superseded by RevolveFeatureData2::Type.

Description

This property gets or sets the
revolution feature type.

Syntax (OLE Automation)

revolveType = RevolveFeatureData.Type  (VB
Get property)

RevolveFeatureData.Type = revolveType  (VB
Set property)

revolveType = RevolveFeatureData.GetType
( ) (C++ Get property)

RevolveFeatureData.SetType ( revolveType
)  (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (int) revolveType | Type of revolution feature:   * 0 = revolve   feature is single directional * 1 = revolve feature is of the midplane type * 2 = revolve feature is bidirectional |

Syntax (COM)

status = RevolveFeatureData ->get\_Type ( &revolveType )

status = RevolveFeatureData ->put\_Type ( revolveType )

|  |  |  |
| --- | --- | --- |
| Property: | (int) revolveType | Type of revolution feature:   * 0 = revolve   feature is single directional * 1 = revolve feature is of the midplane type * 2 = revolve feature is bidirectional |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks