<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetAddToDB.htm -->

# ModelDoc::GetAddToDB

This
method is obsolete and has been superseded by ModelDoc2::GetAddToDB.

Description

This method determines whether or not entities are added directly to
the SolidWorks database.

Syntax (OLE Automation)

retval = ModelDoc.GetAddToDB ()

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) retval | TRUE if adding items directly to the database, FALSE otherwise |

Syntax (COM)

status = ModelDoc->GetAddToDB (
&retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if  adding items directly to the database, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks