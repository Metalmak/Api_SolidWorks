<!-- source: obsoleteapi/PropertyManagerPage2Handler4/PropertyManagerPage2Handler4__OnPopupMenuItem.htm -->

# PropertyManagerPage2Handler4::OnPopupMenuItem

This method is obsolete and has been superseded
by PropertyManagerPage2Handler5::OnPopupMenuItem.

Description

When the user selects a pop-up
menu item, this method determines which item was selected. The add-in
should then perform the appropriate action.

Syntax (OLE Automation)

void = PropertyManagerPage2Handler4.OnPopupMenuItem
( Id)

|  |  |  |
| --- | --- | --- |
| Input: | (long) Id | Unique user-defined ID for a pop-up menu item (see PropertyManagerPage2::AddPopupMenuItem) |

#

Syntax (COM)

status = PropertyManagerPage2Handler4->OnPopupMenuItem
( Id)

|  |  |  |
| --- | --- | --- |
| Input: | (long) Id | Unique user-defined ID for a pop-up menu item (see PropertyManagerPage2::AddPopupMenuItem) |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks