<!-- source: obsoleteapi/SwManipulatorHandler/SwManipulatorHandler__OnItemSetFocus.htm -->

# SwManipulatorHandler::OnItemSetFocus

This method is obsolete and has been superseded
by SwManipulatorHandler2::OnItemSetFocus.

Description

Not currently implemented
for TriadManipulator.

Syntax (OLE Automation)

SwManipulatorHandler.OnItemSetFocus ( pManipulator,
id)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Input: | (int) id | ID of item on which to set focus |

#

Syntax (COM)

status = SwManipulatorHandler->OnItemSetFocus
( pManipulator, id)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Input: | (int) id | ID of item on which to set focus |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks