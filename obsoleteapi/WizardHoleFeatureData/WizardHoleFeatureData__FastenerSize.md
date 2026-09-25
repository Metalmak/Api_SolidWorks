<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__FastenerSize.htm -->

# WizardHoleFeatureData::FastenerSize

This
property is obsolete and has been superseded by WizardHoleFeatureData2::FastenerSize.

Description

This property gets or sets the fastener size
for this wizard hole feature.

Syntax (OLE Automation)

fastenerSize = WizardHoleFeatureData.FastenerSize
( )    (VB Get property)

WizardHoleFeatureData.FastenerSize = fastenerSize   (VB
Set property)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) fastenerSize | Size |

Syntax (COM)

status = WizardHoleFeatureData->get\_FastenerSize
( &fastenerSize ) (COM Get property)

status = WizardHoleFeatureData->put\_FastenerSize
( fastenerSize )  (COM Set property)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) fastenerSize | Size |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks