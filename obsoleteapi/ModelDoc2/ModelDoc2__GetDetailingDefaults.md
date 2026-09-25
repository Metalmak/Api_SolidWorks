<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__GetDetailingDefaults.htm -->

# ModelDoc2::GetDetailingDefaults

This method is obsolete and has been superseded
by ModelDoc2::GetUserPreferenceTextFormat
and ModelDoc2::SetUserPreferenceTextFormat.

Description

This method gets the detailing defaults for this document

Syntax (OLE Automation)

retval = ModelDoc2.GetDetailingDefaults(
)

|  |  |  |
| --- | --- | --- |
| Return: | (LPDISPATCH) retval | Dispatch Pointer for the DetailingDefaults object |

Syntax (COM)

status = ModelDoc2->IGetDetailingDefaults(
&retval )

|  |  |  |
| --- | --- | --- |
| Output: | (LPDETAILINGDEFAULTS) retval | Pointer to the DetailingDefaults object |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks