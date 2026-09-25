<!-- source: obsoleteapi/SheetMetalFeatureData/SheetMetalFeatureData__KFactor.htm -->

(ratio that represents the location of the neutral sheet with respect
to the thickness of the sheet metal part)

# SheetMetalFeatureData::KFactor

This property is obsolete and has been superseded
by SheetMetalFeatureData::GetCustomBendAllowance
and SheetMetalFeatureData::SetCustomBendAllowance.

Description

This property gets or sets the K-Factor
for this sheet metal feature.

Syntax (OLE Automation)

KFactor = SheetMetalFeatureData.KFactor  (
VB Get Property )

SheetMetalFeatureData.KFactor= KFactor  (
VB Set Property )

KFactor  = SheetMetalFeatureData.KFactor   (
C++ Get Property )

SheetMetalFeatureData.KFactor  = KFactor  (
C++ Set Property )

|  |  |  |
| --- | --- | --- |
| Return: | (double) KFactor | K-Factor |

Syntax (COM)

status = SheetMetalFeatureData->get\_KFactor
( &KFactor  )  ( COM Get Property )

status = SheetMetalFeatureData->put\_KFactor
( KFactor  )  ( COM Set Property )

|  |  |  |
| --- | --- | --- |
| Output: | (double) KFactor | K-Factor |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks