<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetVisibilityOfConstructPlanes.htm -->

# ModelDoc::GetVisibilityOfConstructPlanes

This
method is obsolete and has been superseded by ModelDoc2::GetVisibilityOfConstructPlanes.

Description

This method gets whether construction (reference) planes are currently
visible.

Syntax (OLE Automation)

retval = ModelDoc.GetVisibilityOfConstructPlanes
()

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) retval | TRUE if construct planes are currently visible, FALSE if not |

Syntax (COM)

status = ModelDoc->GetVisibilityOfConstructPlanes
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if construct planes are currently visible, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks