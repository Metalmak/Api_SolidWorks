<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__PrintSetup.htm -->

# ModelDoc2::PrintSetup

This
method is obsolete and has been superseded by  ModelDoc2::SetUserPreferenceDoubleValue,
ModelDoc2::SetUserPreferenceIntegerValue,
and ModelDoc2::SetUserPreferenceToggle.

Description

This property gets and sets various parameters
for the current SolidWorks printer.

Syntax (OLE Automation)

setupValue = ModelDoc2.PrintSetup(setupType) (VB
Get property)

ModelDoc2.PrintSetup(setupType) = setupValue (VB
Set property)

setupValue = ModelDoc2.GetPrintSetup
( setupType ) (C++ Get property)

ModelDoc2.SetPrintSetup ( setupType,
setupValue ) (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Input: | (long)setupType | Type of property to set as defined in swPrintProperties\_e |
| Property: | (int) setupValue | Value for property |

Syntax (Com)

status = ModelDoc2->get\_PrintSetup(
setupType, &setupValue )

status = ModelDoc2->put\_PrintSetup(
setupType, setupValue )

|  |  |  |
| --- | --- | --- |
| Input: | (long)setupType | Type of property to set as defined in swPrintProperties\_e |
| Property: | (int) setupValue | Value for property |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

You can use SldWorks::ActivePrinter
to determine or change the current SolidWorks printer.

For information about values for the argument setupValue, see the MSDEV
or Visual Basic Help.