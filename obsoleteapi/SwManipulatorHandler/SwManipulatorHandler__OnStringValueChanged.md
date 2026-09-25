<!-- source: obsoleteapi/SwManipulatorHandler/SwManipulatorHandler__OnStringValueChanged.htm -->

# SwManipulatorHandler::OnStringValueChanged

This method is obsolete and has been superseded
by SwManipulatorHandler2::OnStringValueChanged.

Description

Not currently implemented
for TriadManipulator.

Syntax (OLE Automation)

retVal = SwManipulatorHandler.OnStringValueChanged
( pManipulator, id, value)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Input: | (int) id | ID of the string value to change |
| Input: | (BSTR) value | New string value |
| Output: | (VARIANT\_BOOL) retVal | TRUE if the add-in application accepts the new string value, FALSE if not |

#

Syntax (COM)

status = SwManipulatorHandler->OnStringValueChanged
( pManipulator, id, value, &retVal)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Input: | (int) id | ID of the string value to change |
| Input: | (BSTR) value | New string value |
| Output: | (VARIANT\_BOOL) retVal | TRUE if the add-in application accepts the new string value, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks