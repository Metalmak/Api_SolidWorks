<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__InsertBOMBalloon.htm -->

# ModelDoc2::InsertBOMBalloon

This
method is obsolete and has been superseded by ModelDoc2::InsertBOMBalloon2.

Description

This method inserts a BOM balloon based on
the selected object. The selected object can be an edge, silhouette, face,
or vertex.

Syntax (OLE Automation)

(void) ModelDoc2.InsertBOMBalloon ( )

Syntax (COM)

status = ModelDoc2->InsertBOMBalloon ( )

| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The generated BOM balloon uses the current
settings for:

* Balloon
  style
* Balloon
  fit
* BOM
  balloon upper and lower text (item number, quantity, and custom)