<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-checkin-buildtree-{changesetId}~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/checkin/buildtree/{changesetId} |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Stage Resource Group](PDM%20Pro%20API_ws~g-31fb4871-fcc6-41c5-8856-b0faf87b89f3.html) : api/{vaultName}/checkin/buildtree/{changesetId} (Get) |

Description

Get references tree

Builds a reference tree of files that are uploaded to the specified changeset.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| changesetId | (URI parameter) Changeset ID (required) | integer |
| File | (Response) A FileInfoStageModel object that consists of:     File (File object that consists of FileId (integer) and FileName (string))     Folder (Folder object that consists of FolderId (integer) and FolderPath (string))     Version (integer)     Quantity (integer)     LockedBy (integer)     NewVersion (boolean)     DocumentType (DocumentType object that contains one of:        NoObject = 0        NormalDocument = 1        VirtualComponent = 2        SavedBOM = 3        Item = 4        CutListItem = 5     )     LockViewId (globally unique identifier)     LockProject (integer)     ModifiedDate (date) | FileInfoStageModel |
| IsToolbox | (Response) 1 if a toolbox file, 0 if not | integer |
| ObjectType | (Response) "Folder", "File", or "Bom" | String |

Response (application/json)

Response (text/json)

Response (application/xml)

Response (text/xml)

See Also

[Stage Resource Group](PDM%20Pro%20API_ws~g-31fb4871-fcc6-41c5-8856-b0faf87b89f3.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)