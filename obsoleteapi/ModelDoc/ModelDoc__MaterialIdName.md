<!-- source: obsoleteapi/ModelDoc/ModelDoc__MaterialIdName.htm -->

# ModelDoc::MaterialIdName

This
property is obsolete and has been superseded by ModelDoc2::MaterialIdName.

Description

This property gets and sets the material ID name. This ID is not visible
to the user.

Syntax (OLE Automation)

name = ModelDoc.MaterialIdName (VB
Get property)

ModelDoc.MaterialIdName = name (VB
Set property)

name = ModelDoc.GetMaterialIdName (
) (C++ Get property)

ModelDoc.SetMaterialIdName ( name ) (C++
Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (BSTR) name | Material's ID name property |

Syntax (Com)

status = ModelDoc->get\_MaterialIdName(
&Name )

status = ModelDoc->put\_MaterialIdName(
name )

|  |  |  |
| --- | --- | --- |
| Property: | (BSTR) name | Material's ID name property |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks