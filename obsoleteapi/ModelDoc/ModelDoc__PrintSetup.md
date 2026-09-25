<!-- source: obsoleteapi/ModelDoc/ModelDoc__PrintSetup.htm -->

# ModelDoc::PrintSetup

This
method is obsolete. Use ModelDoc2::SetUserPreferenceDoubleValue,
ModelDoc2::SetUserPreferenceIntegerValue,
and ModelDoc2::SetUserPreferenceToggle.

Description

This property gets and sets various parameters for the current SolidWorks
printer. The current SolidWorks printer can be determined or changed by
calling ModelDoc::ActivePrinter.

Syntax (OLE Automation)

setupValue = ModelDoc.PrintSetup(setupType) (VB
Get property)

ModelDoc.PrintSetup(setupType) = setupValue (VB
Set property)

setupValue = ModelDoc.GetPrintSetup
( setupType ) (C++ Get property)

ModelDoc.SetPrintSetup ( setupType,
setupValue ) (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Input: | (long)setupType | Type of property to set as defined in swPrintProperties\_e |
| Property: | (int) setupValue | Value for property |

Syntax (Com)

status = ModelDoc->get\_PrintSetup(
setupType, &setupValue )

status = ModelDoc->put\_PrintSetup(
setupType, setupValue )

|  |  |  |
| --- | --- | --- |
| Input: | (long)setupType | Type of property to set as defined in swPrintProperties\_e. |
| Property: | (int) setupValue | Value for property |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

For information about values for the argument setupValue, see Visual
Basic online Help topics about printer object constraints.