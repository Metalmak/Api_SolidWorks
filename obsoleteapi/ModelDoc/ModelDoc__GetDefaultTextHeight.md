<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetDefaultTextHeight.htm -->

# ModelDoc::GetDefaultTextHeight

This
method is obsolete and has been superseded by ModelDoc2::GetDefaultTextHeight.

Description

This method returns the default text height in use for this document.

Syntax (OLE Automation)

retval = ModelDoc.GetDefaultTextHeight
()

|  |  |  |
| --- | --- | --- |
| Return: | (double) retval | Default height (in meters) for text in this document |

Syntax (COM)

status = ModelDoc->GetDefaultTextHeight
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (double) retval | Default height (in meters) for text in this document |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks