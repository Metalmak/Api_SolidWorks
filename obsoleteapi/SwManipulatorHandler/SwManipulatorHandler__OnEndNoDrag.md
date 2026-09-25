<!-- source: obsoleteapi/SwManipulatorHandler/SwManipulatorHandler__OnEndNoDrag.htm -->

# SwManipulatorHandler::OnEndNoDrag

This topic is obsolete and has been superseded
by SwManipulatorHandler2::OnEndNoDrag.

Description

This method is called when
a user releases a mouse button and has not dragged the pointer.

Syntax (OLE Automation)

SwManipulatorHandler.OnEndNoDrag ( pManipulator,
handleIndex)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Input: | (int) handleIndex | Control point's handle as defined by swTriadManipulatorControlPoints\_e |

#

Syntax (COM)

status = SwManipulatorHandler->OnEndNoDrag ( pManipulator,
handleIndex)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Input: | (int) handleIndex | Control point's handle as defined by swTriadManipulatorControlPoints\_e |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks