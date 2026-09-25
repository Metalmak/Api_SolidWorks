<!-- source: obsoleteapi/SldWorks/SldWorks__RemoveFileSaveAsItem.htm -->

# SldWorks::RemoveFileSaveAsItem

This method is obsolete and has been superseded
by SldWorks::RemoveFileSaveAsItem2.

Description

This method removes a file type from the
File, Save As list which was added using SldWorks::AddFileSaveAsItem.
The parameters passed to this method should match the parameters you used
when calling SldWorks::AddFileSaveAsItem.

Syntax (OLE Automation)

retval = SldWorks.RemoveFileSaveAsItem
( CallbackFcnAndModule, Description, Type)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) CallbackFcnAndModule | Name of module and function used in your call to AddFileSaveAsItemSldWorks\_AddFileSaveAsItem |
| Input: | (BSTR) Description | Description used in your call to AddFileSaveAsItemSldWorks\_AddFileSaveAsItem |
| Input: | (long) Type | Type of document for the Save As operation as defined in swDocumentTypes\_e |
| Return: | (VARIANT\_BOOL) retval | TRUE if successfully removed from the Save As file type list, FALSE otherwise |

Syntax (COM)

status = SldWorks->RemoveFileSaveAsItem
( CallbackFcnAndModule, Description, Type, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) CallbackFcnAndModule | Name of module and function used in your call to AddFileSaveAsItemSldWorks\_AddFileSaveAsItem |
| Input: | (BSTR) Description | Description used in your call to AddFileSaveAsItemSldWorks\_AddFileSaveAsItem |
| Input: | (long) Type | Type of document for the Save As operation as defined in swDocumentTypes\_e |
| Output: | (VARIANT\_BOOL) retval | TRUE if successfully removed from the Save As file type list, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks