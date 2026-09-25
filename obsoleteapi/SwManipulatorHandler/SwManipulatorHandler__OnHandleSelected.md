<!-- source: obsoleteapi/SwManipulatorHandler/SwManipulatorHandler__OnHandleSelected.htm -->

# SwManipulatorHandler::OnHandleSelected

This method is obsolete and has been superseded
by SwManipulatorHandler2::OnHandleSelected.

Description

Not currently implemented for TriadManipulator.

Syntax (OLE Automation)

SwManipulatorHandler.OnHandleSelected ( pManipulator,
handleIndex )

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Input: | (int) handleIndex | Control point's handle as defined by swTriadManipulatorControlPoints\_e |

#

Syntax (COM)

status = SwManipulatorHandler->OnHandleSelected
( pManipulator, handleIndex )

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Input: | (int) handleIndex | Control point's handle as defined by swTriadManipulatorControlPoints\_e |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks