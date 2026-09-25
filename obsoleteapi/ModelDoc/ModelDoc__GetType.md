<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetType.htm -->

# ModelDoc::GetType

This method is obsolete and has been superseded
by ModelDoc2::GetType.

Description

This method returns the type of the document.

Syntax (OLE Automation)

retval = ModelDoc.GetType ()

|  |  |  |
| --- | --- | --- |
| Return: | (long) retval | Type of document |

Syntax (COM)

status = ModelDoc->GetType ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (long) retval | Type of document |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The document type can be one of the following values:

swDocNONE
- no document

swDocPART
- part document

swDocASSEMBLY-
assembly document

swDocDRAWING
- drawing document

These definitions replace these now obsolete types:

TYPE\_PART
= 1

TYPE\_ASSEMBLY
= 2

TYPE\_DRAWING
= 3