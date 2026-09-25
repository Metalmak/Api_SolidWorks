<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__FileReload.htm -->

# ModelDoc2::FileReload

This
method is obsolete and has been superseded by ModelDoc2::ReloadOrReplace.

Description

This method discards changes and reloads this
model document from disk.

Syntax (OLE Automation)

void ModelDoc2.FileReload ( )

Syntax (COM)

status = ModelDoc2->FileReload ( )

| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This method displays a dialog box in which
the end-user must input data. To avoid the dialog box, use ModelDoc2::ReloadOrReplace.