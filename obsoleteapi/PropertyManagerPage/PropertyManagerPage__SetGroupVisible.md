<!-- source: obsoleteapi/PropertyManagerPage/PropertyManagerPage__SetGroupVisible.htm -->

# PropertyManagerPage::SetGroupVisible

This
object and its methods are obsolete and have been superseded by PropertyManagerPage2.

Description

This method sets whether or not this group
box is visible on this PropertyManager page.

Syntax (OLE Automation)

Not Available.

Syntax (COM)

status = PropertyManagerPage->SetGroupVisible
( GroupId, Visible )

|  |  |  |
| --- | --- | --- |
| Input: | (long) GroupId | Resource ID of the group title's static text control |
| Input: | (VARIANT\_BOOL) Visible | TRUE if the group box is to be visible, otherwise FALSE |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks