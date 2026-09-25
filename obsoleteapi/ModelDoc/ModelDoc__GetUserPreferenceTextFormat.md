<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetUserPreferenceTextFormat.htm -->

# ModelDoc::GetUserPreferenceTextFormat

This
method is obsolete and has been superseded by ModelDoc2::GetUserPreferenceTextFormat.

Description

This method gets the specified text format
user preference from this document.

Syntax (OLE Automation)

retval = ModelDoc.GetUserPreferenceTextFormat ( userPreferenceValue, retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long) userPreferenceValue | User-preference toggle you wish to get; for a complete and up-to-date list of available options, see swUserPreferenceTextFormat\_e |
| Return: | (LPDISPATCH) retval | Pointer to a Dispatch object, the TextFormat object associated with the specified userPreferenceValue setting. |

Syntax (COM)

status = ModelDoc->IGetUserPreferenceTextFormat
( userPreferenceValue, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long) userPreferenceValue | User-pPreference toggle you wish to get; for a complete and up-to-date list of available options, see swUserPreferenceTextFormat\_e |
| Output: | (LPTEXTFORMAT) retval | Pointer to the TextFormat object associated with the specified userPreferenceValue setting |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

This method is the same as using the Tools,
Options menu item.