<!-- source: obsoleteapi/SldWorks/SldWorks__HideToolbar.htm -->

# SldWorks::HideToolbar

This method is obsolete and has been superseded
by SldWorks::HideToolbar2.

Description

This method hides a toolbar that was created with SldWorks::AddToolbar.

Syntax (OLE Automation)

retval = SldWorks.HideToolbar ( moduleName,
toolbarId )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) moduleName | Name of the module (that is, USERDLL) |
| Input: | (long) toolbarId | Toolbar ID |
| Return: | (BOOLEAN) retval | TRUE if successful, FALSE if unsuccessful |

Syntax (COM)

status = SldWorks->HideToolbar (
moduleName, toolbarId, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) moduleName | Name of the module (that is, USERDLL) |
| Input: | (long) toolbarId | Toolbar ID |
| Output: | (VARIANT\_BOOL) retval | TRUE if successful, FALSE if unsuccessful |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks