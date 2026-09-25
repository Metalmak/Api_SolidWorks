<!-- source: obsoleteapi/ModelDoc/ModelDoc__SceneBkgImageFileName.htm -->

# ModelDoc::SceneBkgImageFileName

This property is obsolete
and has been superseded by ModelDoc2::SceneBkgImageFileName.

Description

This property controls the image file name used
as the current background picture.

Syntax (OLE Automation)

Name = ModelDoc.SceneBkgImageFileName (VB
Get property)

ModelDoc.SceneBkgImageFileName
= Name (VB Set property)

Name = ModelDoc.GetSceneBkgImageFileName
( ) (C++ Get property)

ModelDoc.SetSceneBkgImageFileName
( Name ) (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (BSTR) Name | Name of the image file |

Syntax (COM)

status = ModelDoc->get\_SceneBkgImageFileName(
&Name)

status = ModelDoc->put\_SceneBkgImageFileName(
Name )

|  |  |  |
| --- | --- | --- |
| Property: | (BSTR) Name | Name of the image file |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks