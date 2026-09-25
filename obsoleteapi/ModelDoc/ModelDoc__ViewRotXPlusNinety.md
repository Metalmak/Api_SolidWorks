<!-- source: obsoleteapi/ModelDoc/ModelDoc__ViewRotXPlusNinety.htm -->

# ModelDoc::ViewRotXPlusNinety

This method is obsolete
and has been superseded by ModelDoc2::ViewRotXPlusNinety.

Description

This method rotates the view by 90°
about X.

Syntax (OLE Automation)

void ModelDoc.ViewRotXPlusNinety ()

Syntax (COM)

status = ModelDoc->ViewRotXPlusNinety
( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

To increase the speed of dynamic view changes with Hidden Edge or Hidden
Greyed display, use ModelView::StartDynamics and ModelView::StopDynamics.