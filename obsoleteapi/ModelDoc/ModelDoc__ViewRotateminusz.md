<!-- source: obsoleteapi/ModelDoc/ModelDoc__ViewRotateminusz.htm -->

# ModelDoc::ViewRotateminusz

This method is obsolete
and has been superseded by ModelDoc2::ViewRotateminusz.

Description

This method rotates the view around z in a negative direction with the
current increment.

Syntax (OLE Automation)

void ModelDoc.ViewRotateminusz ()

Syntax (COM)

status = ModelDoc->ViewRotateminusz
( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

To increase the speed of dynamic view changes with Hidden Edge or Hidden
Greyed display, use ModelView::StartDynamics and ModelView::StopDynamics.