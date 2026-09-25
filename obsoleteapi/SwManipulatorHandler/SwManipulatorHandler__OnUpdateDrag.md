<!-- source: obsoleteapi/SwManipulatorHandler/SwManipulatorHandler__OnUpdateDrag.htm -->

# SwManipulatorHandler::OnUpdateDrag

This method is obsolete and has been superseded
by SwManipulatorHandler2::OnUpdateDrag.

Description

This method is called when
the pointer moves while the left-mouse or right-mouse button is held down.

Syntax (OLE Automation)

SwManipulatorHandler.OnUpdateDrag ( pManipulator,
handleIndex, newPosMathPt )

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Input: | (int) handleIndex | Control point's handle as defined by swTriadManipulatorControlPoints\_e |
| Input: | (LPDISPATCH) newPosMathPt | Dispatch pointer to the MathPoint object indicating the pointer's new position |

#

Syntax (COM)

status = SwManipulatorHandler->OnUpdateDrag (
pManipulator, handleIndex, newPosMathPt)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Input: | (int) handleIndex | Control point's handle as defined by swTriadManipulatorControlPoints\_e |
| Input: | (LPDISPATCH) newPosMathPt | Dispatch pointer to the MathPoint object indicating the pointer's new position |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks