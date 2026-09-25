<!-- source: obsoleteapi/ModelDoc/ModelDoc__IsExploded.htm -->

# ModelDoc::IsExploded

This
method is obsolete and has been superseded by ModelDoc2::IsExploded.

Description

This method determines if the model is currently exploded.

Syntax (OLE Automation)

retval = ModelDoc.IsExploded ()

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) retval | TRUE if the model is currently displayed in exploded state, FALSE if the model is being displayed in collapsed state |

Syntax (COM)

status = ModelDoc->IsExploded (
&retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the model is currently displayed in exploded state, FALSE if the model is being displayed in collapsed state |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks