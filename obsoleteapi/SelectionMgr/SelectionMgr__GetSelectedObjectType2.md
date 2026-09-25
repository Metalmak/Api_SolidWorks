<!-- source: obsoleteapi/SelectionMgr/SelectionMgr__GetSelectedObjectType2.htm -->

# SelectionMgr::GetSelectedObjectType2

This
method is obsolete and has been superseded by SelectionMgr::GetSelectedObjectType3.

Description

This method gets the type of selected object.

Syntax (OLE Automation)

retval = SelectionMgr.GetSelectedObjectType2
( AtIndex)

|  |  |  |
| --- | --- | --- |
| Input: | (long) AtIndex | Index position within the current list of selected items where AtIndex ranges from 1 to SelectionMgr::GetSelectedObjectCount |
| Return: | (long) retval | Type of object as defined in swSelectType\_e |

Syntax (COM)

status = SelectionMgr->GetSelectedObjectType2
( AtIndex, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long) AtIndex | Index position within the current list of selected items where AtIndex ranges from 1 to SelectionMgr::GetSelectedObjectCount |
| Output: | (long) retval | Type of object as defined in swSelectType\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The index starts at 1, even when using C++.

When reference surfaces are selected in the graphics
view, this method returns swSelFACES instead of the entire swSelREFSURFACES feature.