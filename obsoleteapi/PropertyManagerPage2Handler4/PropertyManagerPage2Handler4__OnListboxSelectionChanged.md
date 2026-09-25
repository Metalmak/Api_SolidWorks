<!-- source: obsoleteapi/PropertyManagerPage2Handler4/PropertyManagerPage2Handler4__OnListboxSelectionChanged.htm -->

# PropertyManagerPage2Handler4::OnListboxSelectionChanged

This method is obsolete and has been superseded
by PropertyManagerPage2Handler5::OnListboxSelectionChanged.

Description

This method is called when
a user changes the selected item in a list box on this PropertyManager.

Syntax (OLE Automation)

void = PropertyManagerPage2Handler4.OnListboxSelectionChanged
( Id, Item )

#

|  |  |  |
| --- | --- | --- |
| Input: | (long) Id | ID of the list box |
| Input: | (long) Item | ID of the item |

#

Syntax (COM)

status = PropertyManagerPage2Handler4->OnListboxSelectionChanged
( Id, Item )

|  |  |  |
| --- | --- | --- |
| Input: | (long) Id | ID of the list box |
| Input: | (long) Item | ID of the item |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks