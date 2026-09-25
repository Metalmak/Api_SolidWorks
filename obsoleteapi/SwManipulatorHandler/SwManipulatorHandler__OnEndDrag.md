<!-- source: obsoleteapi/SwManipulatorHandler/SwManipulatorHandler__OnEndDrag.htm -->

# SwManipulatorHandler::OnEndDrag

This method is obsolete and has been superseded
by SwManipulatorHandler2::OnEndDrag.

Description

This method is called when
a user releases a mouse button after dragging the pointer.

Syntax (OLE Automation)

SwManipulatorHandler.OnEndDrag ( pManipulator)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |

#

Syntax (COM)

status = SwManipulatorHandler->OnEndDrag ( pManipulator)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks