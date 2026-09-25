<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetLayerManager.htm -->

# ModelDoc::GetLayerManager

This
method is obsolete and has been superseded by ModelDoc2::GetLayerManager.

Description

This method returns the LayerMgr object for
the current document. Currently, only drawing documents support this object.

Syntax (OLE Automation)

retval = ModelDoc.GetLayerManager ( )

|  |  |  |
| --- | --- | --- |
| Return: | (LPDISPATCH) retval | Pointer to a Dispatch object, the LayerMgr object for this document |

Syntax (COM)

status = ModelDoc->IGetLayerManager ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (LPLAYERMGR) retval | Pointer to the LayerMgr object for this document |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks