<!-- source: obsoleteapi/ModelDoc/ModelDoc__ViewRotateminusy.htm -->

# ModelDoc::ViewRotateminusy

This method is obsolete
and has been superseded byModelDoc2::ViewRotateminusy.

Description

This function dynamically rotates the view around y in a negative direction
with the current increment.

Syntax (OLE Automation)

void ModelDoc.ViewRotateminusy ()

Syntax (COM)

status = ModelDoc->ViewRotateminusy
( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

To increase the speed of dynamic view changes with Hidden Edge or Hidden
Greyed display, use  ModelView::StartDynamics
and ModelView::StopDynamics.