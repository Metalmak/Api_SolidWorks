<!-- source: obsoleteapi/ModelDoc/ModelDoc__DeleteConfiguration2.htm -->

# ModelDoc::DeleteConfiguration2

This
method is obsolete and has been superseded by ModelDoc2::DeleteConfiguration2.

Description

This method deletes a configuration. The configuration you delete cannot
be the active configuration.

Syntax (OLE Automation)

retval = ModelDoc.DeleteConfiguration2
( configurationName)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) configurationName | Name of the configuration to delete |
| Return: | VARIANT\_BOOL retval | TRUE if successfully deleted, FALSE if not |

Syntax (COM)

status = ModelDoc->DeleteConfiguration2
( configurationName, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) configurationName | Name of the configuration to delete |
| Output: | (VARIANT\_BOOL) retval | TRUE if successfully deleted, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks