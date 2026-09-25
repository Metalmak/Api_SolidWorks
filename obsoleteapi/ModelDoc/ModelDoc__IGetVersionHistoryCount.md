<!-- source: obsoleteapi/ModelDoc/ModelDoc__IGetVersionHistoryCount.htm -->

# ModelDoc::IGetVersionHistoryCount

This
method is obsolete and has been superseded by ModelDoc2::IGetVersionHistoryCount.

Description

This method returns
the size of the array required to hold data returned by [ModelDoc::IVersionHistory](ModelDoc__VersionHistory.htm).

Syntax (OLE Automation)

Not available.

Syntax (COM)

status = ModelDoc->IGetVersionHistoryCount
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (int)retval | Size of array required for the version history |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

If the document has not yet been saved, there is no version history
information and this method will return 0.