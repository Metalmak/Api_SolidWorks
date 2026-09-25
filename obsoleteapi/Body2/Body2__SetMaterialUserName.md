<!-- source: obsoleteapi/Body2/Body2__SetMaterialUserName.htm -->

# Body2::SetMaterialUserName

This method is obsolete and has been superseded
by Body2::SetMaterialUserName2.

Description

This method sets the material user name for this body. This material
name is visible to the user.

Syntax (OLE Automation)

retval = Body2.SetMaterialUserName
( name)

| Input: | (BSTR) name | Material's user name property for this body |
| Return: | (BOOL) retval | TRUE if the material user name was set successfully, FALSE if it was not |

Syntax (COM)

status = Body2->SetMaterialUserName
( name, &retval )

| Input: | (BSTR) name | Material's user name property for this body |
| Output: | (VARIANT\_BOOL) retval | TRUE if the material user name was set successfully, FALSE if it was not |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks