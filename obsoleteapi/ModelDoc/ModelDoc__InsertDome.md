<!-- source: obsoleteapi/ModelDoc/ModelDoc__InsertDome.htm -->

# ModelDoc::InsertDome

This
method is obsolete and has been superseded by ModelDoc2::InsertDome.

Description

This method inserts a dome.

Syntax (OLE Automation)

void ModelDoc.InsertDome ( height,
reverseDir, doEllipticSurface)

|  |  |  |
| --- | --- | --- |
| Input: | (double) height | Height for the dome in meters |
| Input: | (BOOL) reverseDir | TRUE if you want to reverse the dome direction, FALSE otherwise |
| Input: | (BOOL) doEllipticSurface | TRUE if you want the dome to be an elliptical surface, FALSE otherwise |

Syntax (COM)

status = ModelDoc->InsertDome (
height, reverseDir, doEllipticSurface )

|  |  |  |
| --- | --- | --- |
| Input: | (double) height | Hheight for the dome in meters |
| Input: | (VARIANT\_BOOL) reverseDir | TRUE if you want to reverse the dome direction, FALSE otherwise |
| Input: | (VARIANT\_BOOL) doEllipticSurface | TRUE if you want the dome to be an elliptical surface, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks