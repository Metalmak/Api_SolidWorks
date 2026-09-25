<!-- source: obsoleteapi/PropertyManagerPage2Handler4/PropertyManagerPage2Handler4__OnGroupExpand.htm -->

# PropertyManagerPage2Handler4::OnGroupExpand

This method is obsolete and has been superseded
by PropertyManagerPage2Handler5::OnGroupExpand.

Description

This method is called when
a user clicks an arrow to open a group box on the PropertyManager.

Syntax (OLE Automation)

void = PropertyManagerPage2Handler4.OnGroupExpand
( Id, Expanded )

#

|  |  |  |
| --- | --- | --- |
| Input: | (long) Id | ID of the arrow that open a group box |
| Input: | (VARIANT\_BOOL) Expanded | TRUE if the group box is opened, FALSE if not |

#

Syntax (COM)

status = PropertyManagerPage2Handler4->OnGroupExpand
( Id, Expanded )

|  |  |  |
| --- | --- | --- |
| Input: | (long) Id | ID of the arrow that opens a group box |
| Input: | (VARIANT\_BOOL) Expanded | TRUE if the group box is opened, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks