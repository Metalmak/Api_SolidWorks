<!-- source: obsoleteapi/PropertyManagerPage/PropertyManagerPage__GetDialogWindow.htm -->

# PropertyManagerPage::GetDialogWindow

This
object and its methods are obsolete and have been superseded by PropertyManagerPage2.

Description

This method gets
the dialog window to allow access to the dialog controls as necessary.

Syntax (OLE Automation)

Not Available.

Syntax (COM)

status = PropertyManagerPage->GetDialogWindow
( &WindowPtr, &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (long) WindowPtr | Pointer to the dialog's CWnd |
| Output: | (long) retval | Error value |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks