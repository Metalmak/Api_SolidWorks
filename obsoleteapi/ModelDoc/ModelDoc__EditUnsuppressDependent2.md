<!-- source: obsoleteapi/ModelDoc/ModelDoc__EditUnsuppressDependent2.htm -->

# ModelDoc::EditUnsuppressDependent2

This
method is obsolete and has been superseded by ModelDoc2::EditUnsuppressDependent2.

Description

This method unsuppresses the selected feature
or the selected component and any dependents.

Syntax (OLE Automation)

retval = ModelDoc.EditUnsuppressDependent2 ( )

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) retval | TRUE if unsuppress is successful, FALSE otherwise |

Syntax (COM)

status = ModelDoc->EditUnsuppressDependent2 (
VARIANT\_BOOL\* retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if unsuppress is successful, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This routine is identical to ModelDoc::EditUnsuppressDependent.
The version number was incremented to allow VB applications to take advantage
of information not available in PartDoc::EditUnsuppressDependent.