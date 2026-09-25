<!-- source: obsoleteapi/DrawingDocEvents/DrawingDocEvents__ViewNewNotify.htm -->

# ViewNewNotify - DrawingDoc Event

This
event is obsolete and has been superseded by the DrawingDoc event
ViewNewNotify2.

Description

Post-notifies the user program
when the user activates a new view window for the first time.

status = ViewNewNotify ( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

SolidWorks generates this notification
when the user selects Window,
New Window, or uses the splitter
and clicks in the new view.

After you receive notification that the user has
activated a new view for the first time, you can get its handle using
ModelDoc::ActiveView and ModelView::GetViewHWnd.