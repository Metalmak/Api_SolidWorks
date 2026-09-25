<!-- source: obsoleteapi/ModelDoc/ModelDoc__IsEditingSelf.htm -->

# ModelDoc::IsEditingSelf

This method is obsolete
and has been superseded by ModelDoc2::IsEditingSelf.

Description

This method determines if this model is being edited in the context
of another document.

Syntax (OLE Automation)

retval = ModelDoc.IsEditingSelf ()

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) retval | TRUE if this ModelDoc object is the active edit target, FALSE if this ModelDoc object is not the active edit target of the SolidWorks session |

Syntax (COM)

status = ModelDoc->IsEditingSelf
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if this ModelDoc object is the active edit target, FALSE if this ModelDoc object is not the active edit target of the SolidWorks session |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks