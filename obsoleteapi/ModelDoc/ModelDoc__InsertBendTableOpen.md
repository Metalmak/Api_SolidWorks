<!-- source: obsoleteapi/ModelDoc/ModelDoc__InsertBendTableOpen.htm -->

# ModelDoc::InsertBendTableOpen

This method is obsolete
and has been superseded by ModelDoc2::InsertBendTableOpen.

Description

This method inserts an existing bend table
from a file into this model document

Syntax (OLE Automation)

ok = ModelDoc.InsertBendTableOpen ( filename )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) filename | Filename of the bend table you are inserting into this model document |
| Return: | (BOOL) ok | TRUE if the table was successfully inserted, FALSE otherwise |

Syntax (COM)

status = ModelDoc->InsertBendTableOpen ( filename,
&ok )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) filename | Filename of the bend table you are inserting into this model document |
| Output: | (VARIANT\_BOOL) ok | TRUE if the table was successfully inserted, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks