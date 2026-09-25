<!-- source: obsoleteapi/ModelDoc/ModelDoc__Lock.htm -->

# ModelDoc::Lock

This
method is obsolete and has been superseded by ModelDoc2::Lock.

Description

This method blocks the modifying commands in the user interface, effectively
locking the application. This method also changes text on the status bar
to Processing….

Syntax (OLE Automation)

void ModelDoc.Lock ()

Syntax (COM)

status = ModelDoc->Lock ( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Use this method with ModelDoc::UnLock .