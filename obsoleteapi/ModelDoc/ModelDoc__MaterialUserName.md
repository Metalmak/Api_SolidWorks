<!-- source: obsoleteapi/ModelDoc/ModelDoc__MaterialUserName.htm -->

# ModelDoc::MaterialUserName

This
property is obsolete and has been superseded by ModelDoc2::MaterialUserName.

Description

This property gets or sets the material name. This name is visible to
the user in the PhotoWorks product.

Syntax (OLE Automation)

name = ModelDoc.MaterialUserName (VB
Get property)

ModelDoc.MaterialUserName = name (VB
Set property)

name = ModelDoc.GetMaterialUserName
( ) (C++ Get property)

ModelDoc.SetMaterialUserName ( name
) (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (BSTR) name | Material's user name property |

Syntax (Com)

status = ModelDoc->get\_MaterialUserName
( &Name )

status = ModelDoc->put\_MaterialUserName
( name )

|  |  |  |
| --- | --- | --- |
| Property: | (BSTR) name | Material's user name property |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks