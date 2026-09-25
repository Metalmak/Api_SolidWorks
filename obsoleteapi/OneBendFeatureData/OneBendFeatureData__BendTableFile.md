<!-- source: obsoleteapi/OneBendFeatureData/OneBendFeatureData__BendTableFile.htm -->

# OneBendFeatureData::BendTableFile

This property is obsolete and has been
superseded by OneBendFeatureData::GetCustomBendAllowance
and OneBendFeatureData::SetCustomBendAllowance.

Description

This property gets or sets the bend-table pathname
for this bend.

Syntax (OLE Automation)

bendTableFile = OneBendFeatureData.BendTableFile (
VB Get Property )

OneBendFeatureData.BendTableFile = bendTableFile (
VB Set Property )

bendTableFile = OneBendFeatureData.GetBendTableFile (
C++ Get Property )

OneBendFeatureData.SetBendTableFile = bendTableFile (
C++ Set Property )

|  |  |  |
| --- | --- | --- |
| Return: | (BSTR) bendTableFile | Filename for bend table |

Syntax (COM)

status = OneBendFeatureData->get\_BendTableFile
( &bendTableFile) ( COM Get Property )

status = OneBendFeatureData->put\_BendTableFile
( &bendTableFile) ( COM Set Property )

|  |  |  |
| --- | --- | --- |
| Output: | (BSTR) bendTableFile | Filename for bend table |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks