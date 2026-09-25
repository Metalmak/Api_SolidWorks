<!-- source: obsoleteapi/SwManipulatorHandler/SwManipulatorHandler__OnLmbSelected.htm -->

# SwManipulatorHandler::OnLmbSelected

This method is obsolete and has been superseded
by SwManipulatorHandler2::OnLmbSelected.

Description

This method is called when
a user clicks the left-mouse button.

Syntax (OLE Automation)

retVal = SwManipulatorHandler.OnLmbSelected ( pManipulator)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Output: | (VARIANT\_BOOL) retVal | Unknown |

#

Syntax (COM)

status = SwManipulatorHandler->OnLmbSelected (
pManipulator, &retVal)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Output: | (VARIANT\_BOOL) retVal | Unknown |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks