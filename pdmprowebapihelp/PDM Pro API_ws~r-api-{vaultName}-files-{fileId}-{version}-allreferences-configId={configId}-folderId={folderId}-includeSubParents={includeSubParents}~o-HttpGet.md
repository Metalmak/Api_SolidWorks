<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-files-{fileId}-{version}-allreferences-configId={configId}-folderId={folderId}-includeSubParents={includeSubParents}~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/files/{fileId}/{version}/allreferences?configId={configId}&folderId={folderId}&includeSubParents={includeSubParents} |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [File Resource Group](PDM%20Pro%20API_ws~g-20f0f203-5b33-4c77-baf6-4cccf91271c2.html) : api/{vaultName}/files/{fileId}/{version}/allreferences?configId={configId}&folderId={folderId}&includeSubParents={includeSubParents} (Get) |

Description

Get all file references

Gets the reference tree of the specified file.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| fileId | (URI parameter) File ID (required) | integer |
| version | (URI parameter) Version (required) | integer |
| configId | (URI parameter) Config ID (default value is -1) | integer |
| folderId | (URI parameter) Folder ID (default value is 0) | integer |
| includeSubParents | (URI parameter) Whether to include sub parents (default value is false) | boolean |
| File | (Response) A FileInfo object that consists of:  File object that consists of:     FileId (integer)     File Name (string)  Folder object that consists of:     FolderId (integer)     FolderPath  Version (integer)  Config object that consists of :     ConfigurationName (string)     ConfigurationId (integer)    Member of FileRef model | FileInfo |
| IsCyclic | (Response) Whether the file reference is self-referential    Member of FileRef model | boolean |
| IsToolbox | (Response) Whether the file reference is a toolbox item    Member of FileRef model | integer |
| ObjectType | (Response) PweObjectType model; one of:     ObjType\_NoObject = 0     ObjType\_File = 1     ObjType\_InternalComponent = 2     ObjType\_SavedBOM = 3     ObjType\_Item = 4     ObjType\_CutListItem = 5    Member of FileRef model | PweObjectType |
| Warnings | (Response) An array of BaseWarningModels; each BaseWarningModel consists of:     Message  (string)     IsBlocking (boolean)     IsError (boolean)    Member of FileRef model | Collection of BaseWarningModel |
| References | (Response) The file reference's references; an array of FileRefs; each FileRef consists of:     File (FileInfo)     IsCyclic (boolean)     IsToolbox (integer)     ObjectType (PweObjectType)     Warnings (Array of BaseWarningModels)     References (Array of FileRefs)    Member of FileRef model | Collection of FileRef |

Response (application/json)

Response (text/json)

Response (application/xml)

Response (text/xml)

Remarks

This operation can return multiple FileRef objects.

See Also

[File Resource Group](PDM%20Pro%20API_ws~g-20f0f203-5b33-4c77-baf6-4cccf91271c2.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)