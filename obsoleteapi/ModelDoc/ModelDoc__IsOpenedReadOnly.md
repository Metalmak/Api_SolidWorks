<!-- source: obsoleteapi/ModelDoc/ModelDoc__IsOpenedReadOnly.htm -->

# ModelDoc::IsOpenedReadOnly

This
method is obsolete and has been superseded by ModelDoc2::IsOpenedReadOnly.

Description

This method determines if a SolidWorks document is open in read-only
mode.

Syntax (OLE Automation)

retval = ModelDoc.IsOpenedReadOnly
( )

|  |  |  |
| --- | --- | --- |
| Return: | (BOOLEAN) retval | TRUE if this document is read-only, FALSE otherwise |

Syntax (COM)

status = ModelDoc->IsOpenedReadOnly
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if this document is read-only, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks