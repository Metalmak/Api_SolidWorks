<!-- source: obsoleteapi/ModelDoc/ModelDoc__InsertRoutePoint.htm -->

# ModelDoc::InsertRoutePoint

This
method is obsolete and has been superseded by ModelDoc2::InsertRoutePoint.

Description

This method addds a route point based on the
selected point. If the selection set is not complete, then the Insert
Route Point dialog is displayed.

Syntax (OLE Automation)

void ModelDoc.InsertRoutePoint ( )

Syntax (COM)

status = ModelDoc->InsertRoutePoint ( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The route point is the point on the fitting that
aligns with the sketch point when the fitting is inserted.