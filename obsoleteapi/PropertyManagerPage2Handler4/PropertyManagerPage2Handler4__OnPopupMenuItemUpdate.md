<!-- source: obsoleteapi/PropertyManagerPage2Handler4/PropertyManagerPage2Handler4__OnPopupMenuItemUpdate.htm -->

# PropertyManagerPage2Handler4::OnPopupMenuItemUpdate

This method is obsolete and has been superseded
by PropertyManagerPage2Handler5::OnPopupMenuItemUpdate.

Description

When Windows attempts to select
or deselect and enable or disable the pop-up menu item, SolidWorks calls
this method to get the state of the menu item from the add-in. Thus, this
method:

* Processes
  a request for the state of the specified pop-up menu item associated with
  the PropertyManager page.
* Passes
  the state back to SolidWorks.

Syntax (OLE Automation)

void = PropertyManagerPage2Handler4.OnPopupMenuItemUpdate
( Id, Retval)

|  |  |  |
| --- | --- | --- |
| Input: | (long) Id | Unique user-defined ID for a pop-up menu item (see PropertyManagerPage2::AddPopupMenuItem) |
| Input: | (long) Retval | State of the specified unique user-defined pop-up menu item:   * 0 - Not   selected (i.e., not checked) and disabled (i.e., grayed out) * 1 - Not   selected and enabled * 2 - Selected   (i.e., checked) and disabled * 3 - Selected   and enabled |

#

Syntax (COM)

status = PropertyManagerPage2Handler4->OnPopupMenuItemUpdate
( Id, Retval)

|  |  |  |
| --- | --- | --- |
| Input: | (long) Id | Unique user-defined ID for a pop-up menu item (see PropertyManagerPage2::AddPopupMenuItem) |
| Input: | (long) Retval | State of the specified unique user-defined pop-up menu item:   * 0 - Not   selected (i.e., not checked) and disabled (i.e., grayed out) * 1 - Not   selected and enabled * 2 - Selected   (i.e., checked) and disabled * 3 - Selected   and enabled |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks