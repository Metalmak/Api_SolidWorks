<!-- source: obsoleteapi/Body2/Body2__SetMaterialIdName.htm -->

# Body2::SetMaterialIdName

This method is obsolete and has been superseded
by Body2::SetMaterialIdName2.

Description

This method sets the material ID for this body. This value is not visible
to the user.

Syntax (OLE Automation)

retval = Body2.SetMaterialIdName (
name)

| Input: | (BSTR) name | Material's ID name for this body |
| Return: | (BOOL) retval | TRUE if the material ID name was set successfully, FALSE if it was not |

Syntax
(COM)

status = Body2->SetMaterialIdName
( name, &retval )

| Input: | (BSTR) name | Material's ID name for this body |
| Output: | (VARIANT\_BOOL) retval | TRUE if the material ID name was set successfully, FALSE if it was not |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks