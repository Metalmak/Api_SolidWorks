<!-- source: obsoleteapi/SldWorks/SldWorks__NewAssembly.htm -->

# SldWorks::NewAssembly

This method is obsolete and has been superseded
by SldWorks::NewDocument
or SldWorks::INewDocument2.

Description

This method opens a new assembly. The assembly document is named automatically.

Syntax (OLE Automation)

retval = SldWorks.NewAssembly ()

|  |  |  |
| --- | --- | --- |
| Return: | (LPDISPATCH) retval | Pointer to a dispatch object, the newly created assembly or NULL if the operation fails |

Syntax (COM)

status = SldWorks->INewAssembly
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (LPASSEMBLYDOC) retval | Pointer to a newly created assembly or NULL if the operation fails. |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

If you want to set the document title without saving
the file, use ModelDoc2::SetTitle2.