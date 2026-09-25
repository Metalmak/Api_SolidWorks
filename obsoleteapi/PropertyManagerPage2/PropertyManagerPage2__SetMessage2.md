<!-- source: obsoleteapi/PropertyManagerPage2/PropertyManagerPage2__SetMessage2.htm -->

# PropertyManagerPage2::SetMessage2

This method is obsolete and has been superseded
by PropertyManagerPage2::SetMessage3.

Description

This method sets the message in this PropertyManager
page.

Syntax (OLE Automation)

retval = PropertyManagerPage2.SetMessage2 ( Message,
Visibility, Caption )

#

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) Message | Message text |
| Input: | (long) Visibility | Visibility state of this message as defined by swPropertyManagerPageMessageVisibility |
| Input: | (BSTR) Caption | Caption for message |
| Output: | (VARIANT\_BOOL) retval | TRUE if the message is set, FALSE if not |

#

Syntax (COM)

status = PropertyManagerPage2->SetMessage2 ( Message,
Visibility, Caption, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) Message | Message text |
| Input: | (long) Visibility | Visibility state of this message as defined by swPropertyManagerPageMessageVisibility |
| Input: | (BSTR) Caption | Caption for message |
| Output: | (VARIANT\_BOOL) retval | TRUE if the message is set, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks

If Caption is empty, then
the current caption is not changed.

This method should be useful
when creating multipage PropertyManager pages where you want different
informational messages on each page.