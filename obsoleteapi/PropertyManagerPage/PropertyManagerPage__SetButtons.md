<!-- source: obsoleteapi/PropertyManagerPage/PropertyManagerPage__SetButtons.htm -->

# PropertyManagerPage::SetButtons

This
object and its methods are obsolete and have been superseded by PropertyManagerPage2.

Description

This method adds a generic
button to top of the PropertyManager page.

Syntax (OLE Automation)

Not Available.

Syntax (COM)

status = PropertyManagerPage->SetButtons ( ButtonTypes,
&retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long) ButtonTypes | Button types to add to the top of the PropertyManager page as defined in swPropertyManagerButtonTypes\_e |
| Output: | (long) retval | Error values as defined in swPropertyManagerStatus\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks