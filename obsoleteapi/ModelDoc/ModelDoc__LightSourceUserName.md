<!-- source: obsoleteapi/ModelDoc/ModelDoc__LightSourceUserName.htm -->

# ModelDoc::LightSourceUserName

This property is obsolete
and has been superseded by ModelDoc2::LightSourceUserName.

Description

This property gets or sets the light source name that is displayed in
the SolidWorks user interface.

Syntax (OLE Automation)

Name = ModelDoc.LightSourceUserName(
id ) (VB Get property)

ModelDoc.LightSourceUserName( id )
= Name (VB Set property)

newName = ModelDoc.GetLightSourceUserName
( id, ) (C++ Get property)

ModelDoc.SetLightSourceUserName ( id,
newName ) (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Input | (long) id | Light source ID |
| Property: | (BSTR) Name | Name to give to the light source |

Syntax (Com)

status = ModelDoc->get\_LightSourceUserName(
id, &Name)

status = ModelDoc->put\_GetLightSourceUserName(
id, Name )

|  |  |  |
| --- | --- | --- |
| Input | (long) id | Light source ID |
| Property: | (BSTR) Name | Name to give to the light source |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The light source ID ranges from 0 to n,
where n = (the total number of
light sources - 1). To get the total number of light sources, use ModelDoc::GetLightSourceCount.