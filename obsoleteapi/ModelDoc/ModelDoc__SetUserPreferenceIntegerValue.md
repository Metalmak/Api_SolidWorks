<!-- source: obsoleteapi/ModelDoc/ModelDoc__SetUserPreferenceIntegerValue.htm -->

# ModelDoc::SetUserPreferenceIntegerValue

This method is obsolete
and has been superseded by ModelDoc2::SetUserPreferenceIntegerValue.

Description

This method sets various user preference integer values.

Syntax (OLE Automation)

retval = ModelDoc.SetUserPreferenceIntegerValue ( userPreferenceValue, value )

|  |  |  |
| --- | --- | --- |
| Input: | (long) userPreferenceValue | Toggle to change as defined by swUserPreferenceIntegerValue\_e |
| Input: | (long) value | Numeric value to give to the user preference specified in userPreferenceValue |
| Return: | (BOOL) retval | TRUE if the setting was changed successfully, FALSE otherwise |

Syntax (COM)

status = ModelDoc->SetUserPreferenceIntegerValue
( userPreferenceValue, value, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long) userPreferenceValue | Toggle to change as defined by swUserPreferenceIntegerValue\_e |
| Input: | (long) value | Numeric value to give to the user preference specified in userPreferenceValue |
| Output: | (VARIANT\_BOOL) retval | TRUE if the setting was changed successfully, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks