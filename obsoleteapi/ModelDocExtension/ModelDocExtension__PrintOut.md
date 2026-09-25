<!-- source: obsoleteapi/ModelDocExtension/ModelDocExtension__PrintOut.htm -->

# ModelDocExtension::PrintOut

This method is obsolete and has been superseded
by ModelDocExtension::PrintOut2.

Description

This method prints the document with options
and without any dialogs or message boxes

Syntax (OLE Automation)

void ModelDocExtension.PrintOut ( FromPage, ToPage,
Copies, Collate, Printer, PrintFileName )

#

|  |  |  |
| --- | --- | --- |
| Input: | (long) FromPage | First page in the range of pages to print |
| Input: | (long) ToPage | Last page in the range of pages to print |
| Input: | (long) Copies | Number of copies to print |
| Input: | (VARIANT\_BOOL) Collate | TRUE collates the copies, FALSE does not |
| Input: | (BSTR) Printer | Name of the printer queue; if you pass a NULL string, then this method prints to the current SolidWorks printer; you can use ModelDoc2::Printer to set the current SolidWorks printer |
| Input: | (BSTR) PrintFileName | Name of the file to print to |

#

Syntax (COM)

status = ModelDocExtension->PrintOut ( FromPage,
ToPage, Copies, Collate, Printer, PrintFileName )

|  |  |  |
| --- | --- | --- |
| Input: | (long) FromPage | First page in the range of pages to print |
| Input: | (long) ToPage | Last page in the range of pages to print |
| Input: | (long) Copies | Number of copies to print |
| Input: | (VARIANT\_BOOL) Collate | TRUE collates the copies, FALSE does not |
| Input: | (BSTR) Printer | Name of the printer queue; if you pass a NULL string, then this method prints to the current SolidWorks printer; you can use ModelDoc2::Printer to set the current SolidWorks printer |
| Input: | (BSTR) PrintFileName | Name of the file to print to |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks

This method supports printing
parts, assemblies, and both single and multisheet drawings. No dialogs
or message boxes are displayed.