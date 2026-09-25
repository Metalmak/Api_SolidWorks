<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__EditUnsuppressDependent.htm -->

# ModelDoc2::EditUnsuppressDependent

This
method is obsolete and has been superseded by ModelDoc2::EditUnsuppressDependent2.

Description

This method unsuppresses the selected feature
or the selected component and any  dependents.

Syntax (OLE Automation)

retval = ModelDoc2.EditUnsuppressDependent ( )

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) retval | TRUE if unsuppressed, FALSE otherwise |

Syntax (COM)

status = ModelDoc2->EditUnsuppressDependent (
&retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if unsuppressed, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks