<!-- source: obsoleteapi/Component/Component__GetMaterialIdName.htm -->

# Component::GetMaterialIdName

This
method is obsolete and has been superseded by Component2::GetMaterialIdName.

Description

This method gets the identifying name of the material for this component
object.

Syntax (OLE Automation)

retval
= Component.GetMaterialIdName ()

| Return: | (BSTR) retval | Material ID |

Syntax (COM)

status
= Component->GetMaterialIdName ( &retval )

| Output: | (BSTR) retval | Material ID |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks