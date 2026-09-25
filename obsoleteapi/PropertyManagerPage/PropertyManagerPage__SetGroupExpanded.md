<!-- source: obsoleteapi/PropertyManagerPage/PropertyManagerPage__SetGroupExpanded.htm -->

# PropertyManagerPage::SetGroupExpanded

This
object and its methods are obsolete and have been superseded by PropertyManagerPage2.

Description

This method sets whether or not this group
box is expanded on this PropertyManager page.

Syntax (OLE Automation)

Not Available.

Syntax (COM)

status = PropertyManagerPage->SetGroupExpanded
( GroupId, Expanded )

|  |  |  |
| --- | --- | --- |
| Input: | (long) GroupId | Resource ID of the group title's static text control |
| Input: | (VARIANT\_BOOL) Expanded | TRUE if the group box is to be expanded, otherwise FALSE |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks