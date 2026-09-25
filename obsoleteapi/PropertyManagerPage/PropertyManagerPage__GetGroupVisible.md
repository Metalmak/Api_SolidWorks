<!-- source: obsoleteapi/PropertyManagerPage/PropertyManagerPage__GetGroupVisible.htm -->

# PropertyManagerPage::GetGroupVisible

This
object and its methods are obsolete and have been superseded by PropertyManagerPage2.

Description

This method gets whether or not this group
box is visible on this PropertyManager page.

Syntax (OLE Automation)

Not Available.

Syntax (COM)

status = PropertyManagerPage->GetGroupVisible
( GroupId, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long) GroupId | Resource ID of the group title's static text control |
| Output: | (VARIANT\_BOOL) retval | TRUE if the group box is visible, otherwise FALSE |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks