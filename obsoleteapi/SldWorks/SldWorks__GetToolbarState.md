<!-- source: obsoleteapi/SldWorks/SldWorks__GetToolbarState.htm -->

# SldWorks::GetToolbarState

This method is obsolete and has been superseded
by SldWorks::GetToolbarState2.

Description

This method returns the state of a toolbar.

Syntax (OLE Automation)

retval = SldWorks.GetToolbarState (
Module, toolbarID, toolbarState )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) Module | Name of the module (for example, USERDLL) |
| Input: | (long) toolbarID | Toolbar ID |
| Input: | (long) toolbarState | Toolbar state as defined in swToolbarStates\_e |
| Return: | (Boolean)retval | TRUE or FALSE based on toolbarState |

Syntax (COM)

status = SldWorks->GetToolbarState
( Module, toolbarID, toolbarState, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR)Module | Name of the module (for example, USERDLL) |
| Input: | (long)toolbarID | Toolbar ID |
| Input: | (long)toolbarState | Toolbar state as defined in swToolbarStates\_e |
| Output: | (VARIANT\_BOOL)retval | TRUE or FALSE based on toolbarState |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

You can determine if a toolbar is hidden by passing swToolbarHidden
in toolbarState.