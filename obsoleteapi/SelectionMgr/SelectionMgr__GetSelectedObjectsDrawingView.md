<!-- source: obsoleteapi/SelectionMgr/SelectionMgr__GetSelectedObjectsDrawingView.htm -->

# SelectionMgr::GetSelectedObjectsDrawingView

This method is obsolete and has been superseded
by SelectionMgr::GetSelectedObjectsDrawingView2.

Description

This method gets the drawing view for the selected
object.

Syntax (OLE Automation)

retval = SelectionMgr.GetSelectedObjectsDrawingView
( atIndex)

|  |  |  |
| --- | --- | --- |
| Input: | (long) atIndex | Index position within the current list of selected items where AtIndex ranges from 1 to SelectionMgr::GetSelectedObjectCount |
| Output: | (LPVIEW) drView | Pointer to the drawing view |

Syntax (COM)

status = SelectionMgr->GetSelectedObjectsDrawingView
( atIndex, &drView )

|  |  |  |
| --- | --- | --- |
| Input: | (long) atIndex | Index position within the current list of selected items where AtIndex ranges from 1 to SelectionMgr::GetSelectedObjectCount |
| Output: | (LPVIEW) drView | Pointer to the drawing view |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks