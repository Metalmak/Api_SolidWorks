<!-- source: obsoleteapi/Component/Component__GetMaterialUserName.htm -->

# Component::GetMaterialUserName

This method is obsolete and has been superseded by Component2::GetMaterialUserName.

Description

This method gets the user-visible name of the material for this component
object.

Syntax (OLE Automation)

retval
= Component.GetMaterialUserName ()

| Return: | (BSTR) retval | Material user name property |

Syntax (COM)

status = Component->GetMaterialUserName
( &retval )

| Output: | (BSTR) retval | Material user name property |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks