<!-- source: obsoleteapi/ModelDoc/ModelDoc__DeleteNamedView.htm -->

# ModelDoc::DeleteNamedView

This
method is obsolete and has been superseded by ModelDoc2::DeleteNamedView.

Description

This method deletes the specified model view.

Syntax (OLE Automation)

retval = ModelDoc.DeleteNamedView (
viewname)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) viewname | Name of the view you wish to delete |
| Return: | (BOOL) retval | TRUE if the view was deleted successfully, FALSE if not |

Syntax (COM)

status = ModelDoc->DeleteNamedView
( viewname, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) viewname | Name of the view you wish to delete |
| Output: | (VARIANT\_BOOL) retval | TRUE if the view was deleted successfully, if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks