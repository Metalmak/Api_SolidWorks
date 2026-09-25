<!-- source: obsoleteapi/ModelDoc/ModelDoc__IRelease3rdPartyStorage.htm -->

# ModelDoc::IRelease3rdPartyStorage

This
method is obsolete and has been superseded by ModelDoc2::IRelease3rdPartyStorage.

Description

This method
closes the specified storage stream.

Syntax (OLE Automation)

Not Available.

Syntax (COM)

status = ModelDoc-> IRelease3rdPartyStorage(
stringIn )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) stringIn | Name of the storage stream to close |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

Use this method with [ModelDoc::IGet3rdPartyStorage](ModelDoc__IGet3rdPartyStorage.htm)
f you are not using the LoadFromStorageNotify event. You need must call
this method even when the call to ModelDoc::IGet3rdPartyStorage returns
a NULL stream. For more information, see ModelDoc::IGet3rdPartyStorage.

NOTE:
If you are using serialization, then you should be careful with
the standard MFC macros; otherwise, you might get messages like Unexpected File Format after your application
is unloaded. One way of using IMPLEMENT\_SERIAL is:

IMPLEMENT\_SERIAL( CCustomAttr, CObject, VERSIONABLE\_SCHEMA|0 )