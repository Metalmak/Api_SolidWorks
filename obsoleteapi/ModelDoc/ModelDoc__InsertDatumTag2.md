<!-- source: obsoleteapi/ModelDoc/ModelDoc__InsertDatumTag2.htm -->

# ModelDoc::InsertDatumTag2

This
method is obsolete and has been superseded by ModelDoc2::InsertDatumTag2.

Description

This method inserts a datum tag symbol at the
selected location.

Syntax (OLE Automation)

retval = ModelDoc.InsertDatumTag2 ( )

|  |  |  |
| --- | --- | --- |
| Return: | (LPDISPATCH) retval | Pointer to a Dispatch object, the newly created DATUMTAG object |

Syntax (COM)

status = ModelDoc->IInsertDatumTag2 ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (LPDATUMTAG) retval | Pointer to a newly created LPDATUMTAG object |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks