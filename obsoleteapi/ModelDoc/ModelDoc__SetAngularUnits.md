<!-- source: obsoleteapi/ModelDoc/ModelDoc__SetAngularUnits.htm -->

# ModelDoc::SetAngularUnits

This
method is obsolete and has been superseded by ModelDoc2::SetAngularUnits.

Description

This method sets the current angular units.

Syntax (OLE Automation)

void ModelDoc.SetAngularUnits ( uType,
fractBase, fractDenom, sigDigits)

|  |  |  |
| --- | --- | --- |
| Input: | (short) uType | Angular units as defined in swAngleUnit\_e |
| Input: | (short) fractBase | Not used; input to this field is required, but is not used |
| Input: | (short) fractDenom | Not used; input to this field is required but is not used |
| Input: | (short) sigDigits | Significant digits if using decimal units |

Syntax (COM)

status = ModelDoc->SetAngularUnits
( uType, fractBase, fractDenom, sigDigits )

|  |  |  |
| --- | --- | --- |
| Input: | (short) uType | Angular units as defined in swAngleUnit\_e |
| Input: | (short) fractBase | Not used; input to this field is required but is not used |
| Input: | (short) fractDenom | Not used; input to this field is required but is not used |
| Input: | (short) sigDigits | Significant digits if using decimal units |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks