<!-- source: obsoleteapi/ModelDoc/ModelDoc__SceneUserName.htm -->

# ModelDoc::SceneUserName

This property is obsolete
and has been superseded by ModelDoc2::SceneUserName.

Description

The method gets and sets the scene user name.

Syntax (OLE Automation)

newName = ModelDoc.SceneUserName (VB
Get property)

ModelDoc.SceneUserName = Name (VB
Set property)

newName = ModelDoc.GetSceneUserName
( ) (C++ Get property)

ModelDoc.SetSceneUserName ( Name ) (C++
Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (BSTR) Name | User name of the scene |

Syntax (COM)

status = ModelDoc->get\_SceneUserName(
&Name )

status = ModelDoc->put\_SceneUserName(
Name )

|  |  |  |
| --- | --- | --- |
| Property: | (BSTR) Name | User name of the scene |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks