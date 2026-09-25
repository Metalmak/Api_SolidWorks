<!-- source: obsoleteapi/SldWorks/SldWorks__RemoveUserMenu.htm -->

# SldWorks::RemoveUserMenu

This
method is obsolete and has been superseded by SldWorks::RemoveMenu.

Description

This method removes the menu item or shortcut menu associated with the
specified unique menu ID. By specifying the menu ID, you can remove a
blank menu item.

Syntax (OLE Automation)

retval = SldWorks.RemoveUserMenu (
docType, menuIdIn, moduleName )

|  |  |  |
| --- | --- | --- |
| Input: | (long) docType | Type of document to which this menu item had been added |
| Input: | (long) menuIdIn | The ID of the menu item to remove; this menu ID is the same ID returned from your call to SldWorks::AddMenuItem2 or SldWorks::AddMenuPopupItem |
| Input: | (BSTR) moduleName | Name of the module (for example, USERDLL) |
| Return: | (VARIANT\_BOOLEAN) retval | TRUE if successful, FALSE if unsuccessful |

Syntax (COM)

status = SldWorks->RemoveUserMenu
( docType, menuIdIn, moduleName, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long) docType | Type of document to which this menu item had been added |
| Input: | (long) menuIdIn | The ID of the menu item to remove; this menu ID is the same ID returned from your call to SldWorks::AddMenuItem2 or SldWorks::AddMenuPopupItem |
| Input: | (BSTR) moduleName | Name of the module (for example, USERDLL) |
| Output: | (VARIANT\_BOOL) retval | TRUE if successful, FALSE if unsuccessful |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks