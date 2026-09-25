<!-- source: obsoleteapi/SwManipulatorHandler/SwManipulatorHandler__OnDoubleValueChanged.htm -->

# SwManipulatorHandler::OnDoubleValueChanged

This method is obsolete and was superseded
by SwManipulatorHandler2::OnDoubleValueChanged.

Description

Not currently implemented
for TriadManipulator.

Syntax (OLE Automation)

retVal = SwManipulatorHandler.OnDoubleValueChanged
( pManipulator, id, value)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Input: | (int) id | ID of the double value to change |
| Input: | (double) value | New double value |
| Output: | (VARIANT\_BOOL) retVal | TRUE if the add-in application accepts the new double value, FALSE if not |

#

Syntax (COM)

status = SwManipulatorHandler->OnDoubleValueChanged
( pManipulator, id, value, &retVal)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Input: | (int) id | ID of the double value to change |
| Input: | (double) value | New double value |
| Output: | (VARIANT\_BOOL) retVal | TRUE if the add-in application accepts the new double value, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks