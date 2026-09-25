<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__EditSuppress.htm -->

# ModelDoc2::EditSuppress

This method is obsolete and has been superseded
by ModelDoc2::EditSuppress2.

Description

This method suppresses the selected feature,
the selected component, or the owning feature of the selected face.

Syntax (OLE Automation)

retval = ModelDoc2.EditSuppress ( )

| Return: | (BOOL) retval | TRUE if suppressed, FALSE otherwise |

Syntax (COM)

status = ModelDoc2->EditSuppress ( &retval
)

| Output: | (VARIANT\_BOOL) retval | TRUE if suppressed, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks