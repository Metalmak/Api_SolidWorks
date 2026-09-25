<!-- source: obsoleteapi/ModelDoc/ModelDoc__IsLightLockedToModel.htm -->

# ModelDoc::IsLightLockedToModel

This
method is obsolete and has been superseded by ModelDoc2::IsLightLockedToModel.

Description

This method determines if the specified light
is fixed.

Syntax (OLE Automation)

retval = ModelDoc.IsLightLockedToModel ( lightId )

|  |  |  |
| --- | --- | --- |
| Input: | (long)lightId | Lght ID |
| Return: | (BOOL) retval | TRUE if the light is fixed, FALSE otherwise |

Syntax (COM)

status = ModelDoc->IsLightLockedToModel ( lightId,
&retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long)lightId | Light ID |
| Output: | (VARIANT\_BOOL) retval | TRUE if the light is fixed, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks