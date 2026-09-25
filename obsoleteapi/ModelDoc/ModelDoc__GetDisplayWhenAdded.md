<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetDisplayWhenAdded.htm -->

# ModelDoc::GetDisplayWhenAdded

This
method is obsolete and has been superseded by ModelDoc2::GetDisplayWhenAdded.

Description

This method determines whether entities are displayed when created.

Syntax (OLE Automation)

retval = ModelDoc.GetDisplayWhenAdded
()

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) retval | TRUE if new entities are displayed when added, FALSE if not |

Syntax (COM)

status = ModelDoc->GetDisplayWhenAdded
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if new entities are displayed when added, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks