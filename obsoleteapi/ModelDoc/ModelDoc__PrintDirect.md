<!-- source: obsoleteapi/ModelDoc/ModelDoc__PrintDirect.htm -->

# ModelDoc::PrintDirect

This
method is obsolete and has been superseded by ModelDoc2::PrintDirect.

Description

This method prints the current document to the default printer.

Syntax (OLE Automation)

void ModelDoc.PrintDirect ()

Syntax (COM)

status = ModelDoc->PrintDirect (
)

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

For a drawing document, all sheets are printed. For a part or assembly
document, the currently active view is printed.