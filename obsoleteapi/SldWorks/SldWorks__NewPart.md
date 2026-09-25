<!-- source: obsoleteapi/SldWorks/SldWorks__NewPart.htm -->

# SldWorks::NewPart

This
method is obsolete and has been superseded by SldWorks::NewDocument or SldWorks::INewDocument2.

Description

This method opens a new part and names it automatically.

Syntax (OLE Automation)

retval = SldWorks.NewPart ()

|  |  |  |
| --- | --- | --- |
| Return: | (LPDISPATCH) retval | Pointer to a dispatch object, the newly created part or NULL if the operation fails |

Syntax (COM)

status = SldWorks->INewPart ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (LPPARTDOC) retval | Pointer to the newly created part or NULL if the operation fails. |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

If you want to set the document title without saving
the file, use ModelDoc2::SetTitle2.