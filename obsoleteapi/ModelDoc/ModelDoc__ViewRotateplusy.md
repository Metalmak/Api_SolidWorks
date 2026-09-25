<!-- source: obsoleteapi/ModelDoc/ModelDoc__ViewRotateplusy.htm -->

# ModelDoc::ViewRotateplusy

This method is obsolete
and has been superseded by ModelDoc2::ViewRotateplusy.

Description

This method rotates the view around y in a positive direction with the
current increment.

Syntax (OLE Automation)

void ModelDoc.ViewRotateplusy ()

Syntax (COM)

status = ModelDoc->ViewRotateplusy
( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

To increase the speed of dynamic view changes with Hidden Edge or Hidden
Greyed display, use  ModelView::StartDynamics
and ModelView::StopDynamics.