<!-- source: obsoleteapi/ModelDoc/ModelDoc__ViewRotYMinusNinety.htm -->

# ModelDoc::ViewRotYMinusNinety

This method is obsolete
and has been superseded by ModelDoc2::ViewRotYMinusNinety.

Description

This method dynamically rotates the view by -90°
about Y.

Syntax (OLE Automation)

void ModelDoc.ViewRotYMinusNinety ()

Syntax (COM)

status = ModelDoc->ViewRotYMinusNinety
( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) tatus | S\_OK if successful |

Remarks

To increase the speed of dynamic view changes with Hidden Edge or Hidden
Greyed display, use ModelView::StartDynamics and ModelView::StopDynamics.