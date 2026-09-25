<!-- source: obsoleteapi/RevolveFeatureData/RevolveFeatureData__IsBossFeature.htm -->

# RevolveFeatureData::IsBossFeature

This
method is obsolete and has been superseded by RevolveFeatureData2::IsBossFeature.

Description

This method gets whether the revolution is
a boss feature.

Syntax (OLE Automation)

isBossFeature = RevolveFeatureData.IsBossFeature
( )

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) isBossFeature | TRUE if revolution is a boss feature, FALSE if not |

Syntax (COM)

status = RevolveFeatureData ->IsBossFeature (
&isBossFeature )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) isBossFeature | TRUE if revolution is a boss feature, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks