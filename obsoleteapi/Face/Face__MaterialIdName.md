<!-- source: obsoleteapi/Face/Face__MaterialIdName.htm -->

# Face::MaterialIdName

This
property is obsolete and has been superseded by Face2::MaterialIdName.

Description

This property gets or sets the material ID name. This ID is not visible
to the user.

Syntax (OLE Automation)

name
= Face.MaterialIdName (VB Get property)

Face.MaterialIdName
= name (VB Set property)

name
= Face.GetMaterialIdName ( ) (C++ Get property)

Face.SetMaterialIdName
( name ) (C++ Set property)

| Property: | (BSTR) name | Material ID name property on the individual face |

Syntax (COM)

status
= Face->get\_MaterialIdName(&name)

status
= Face->put\_MaterialIdName(name)

| Property: | (BSTR) name | Material ID name property on the individual face |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Please note that this property is currently unsupported for faces obtained
from reference surface bodies.