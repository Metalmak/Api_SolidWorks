<!-- source: obsoleteapi/SldWorks/SldWorks__SetToolbarDock.htm -->

# SldWorks::SetToolbarDock

This method is obsolete and has been superseded
by SldWorks::SetToolbarDock2.

Description

This method sets the docking state of the toolbar.

Syntax (OLE Automation)

void SldWorks.SetToolbarDock (Module, ToolbarID,
DockState )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) Module | Name of the module (that is, USERDLL) |
| Input: | (long) ToolbarID | ID of the Toolbar |
| Input: | (long) DockState | Docking state of the toolbar as defined in  swToolbarDockStatePosition\_e |

Syntax (COM)

status = SldWorks->SetToolbarDock ( Module, ToolbarID,
DockState )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) Module | Name of the module (that is, USERDLL) |
| Input: | (long) ToolbarID | ID of the Toolbar |
| Input: | (long) DockState | Docking state of the toolbar as defined in  swToolbarDockStatePosition\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks