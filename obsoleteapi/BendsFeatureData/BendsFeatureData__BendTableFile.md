<!-- source: obsoleteapi/BendsFeatureData/BendsFeatureData__BendTableFile.htm -->

# BendsFeatureData::BendTableFile

This property is obsolete and has been
superseded by BendsFeatureData::GetCustomBendAllowance
and BendsFeatureData::SetCustomBendAllowance.

Description

This property gets or sets the path for the
bend table for this Flatten-Bends/Process-Bends feature.

Syntax (OLE Automation)

bendTableFile = BendsFeatureData.BendTableFile  (
VB Get Property )

BendsFeatureData.BendTableFile = bendTableFile  (
VB Set Property )

bendTableFile = BendsFeatureData.get\_BendTableFile  (
C++ Get Property )

BendsFeatureData.BendTableFile = put\_bendTableFile  (
C++ Set Property )

|  |  |  |
| --- | --- | --- |
| Return: | (BSTR) bendTableFile | File name of the bend table |

Syntax (COM)

status = BendsFeatureData->get\_BendTableFile (
&bendTableFile)  ( COM Get Property )

status = BendsFeatureData->put\_BendTableFile (
bendTableFile)  ( COM Set Property )

|  |  |  |
| --- | --- | --- |
| Output: | (BSTR) bendTableFile | File name of the bend table |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks