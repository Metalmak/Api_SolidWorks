<!-- source: obsoleteapi/PropertyManagerPage2Handler/PropertyManagerPage2Handler__OnHelp.htm -->

# PropertyManagerPage2Handler::OnHelp

This method is obsolete and has been superseded
by [PropertyManagerPage2Handler2::OnHelp](../PropertyManagerPage2Handler2/PropertyManagerPage2Handler2__OnHelp.htm).

Description

This method is called when the end-user clicks
a Help button in this PropertyManager.

Syntax (OLE Automation)

retval = PropertyManagerPage2Handler.OnHelp ( )

#

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the help file opens successfully, FALSE if not |

#

Syntax (COM)

status = PropertyManagerPage2Handler->OnHelp (
&retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the help file opens successfully, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks