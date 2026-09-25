<!-- source: obsoleteapi/SwManipulatorHandler/SwManipulatorHandler__OnDelete.htm -->

# SwManipulatorHandler::OnDelete

This method is obsolete and has been superseded
by SwManipulatorHandler2::OnDelete.

Description

This method is called when
the SolidWorks document is closed.

Syntax (OLE Automation)

retVal = SwManipulatorHandler.OnDelete ( pManipulator)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Output: | (VARIANT\_BOOL) retVal | TRUE if the add-in application deletes the manipulator, FALSE if not |

#

Syntax (COM)

status = SwManipulatorHandler->OnDelete ( pManipulator,
&retVal)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) pManipulator | Dispatch pointer to the Manipulator object |
| Output: | (VARIANT\_BOOL) retVal | TRUE if the add-in application deletes the manipulator, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks