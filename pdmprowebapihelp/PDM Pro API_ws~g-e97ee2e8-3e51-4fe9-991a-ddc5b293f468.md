<!-- source: pdmprowebapihelp/PDM Pro API_ws~g-e97ee2e8-3e51-4fe9-991a-ddc5b293f468.html -->

PDM Pro API Web Service

Stage Resource Group

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) : Stage Resource Group |

Description

Consists of APIs for changeset management such as adding files to the vault and other check-in operations.

Operations

|  |  |
| --- | --- |
| Get | [api/{vaultName}/changeset/create](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-changeset-create~o-HttpGet.html) GET: api/{vaultName}/changeset/create Generate changesetId   Gets a changeset ID for the specified vault. |
| Put | [api/{vaultName}/checkin/{changesetId}/{overrideVersion}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-checkin-%7BchangesetId%7D-%7BoverrideVersion%7D~o-HttpPut.html) PUT: api/{vaultName}/checkin/{changesetId}/{overrideVersion=false} Check in files from the changeset   Checks in the specified changeset. |
| Put | [api/{vaultName}/checkin/addfiles/{changesetId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-checkin-addfiles-%7BchangesetId%7D~o-HttpPut.html) PUT: api/{vaultname}/checkin/addfiles/{changesetId=0} Upload files or document ids to changeset to the check in operation   Uploads files to the specified changeset for checkin. |
| Get | [api/{vaultName}/checkin/buildtree/{changesetId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-checkin-buildtree-%7BchangesetId%7D~o-HttpGet.html) GET: api/{vaultName}/checkin/buildtree/{changesetId} Get references tree   Builds a reference tree of files that are uploaded to the specified changeset. |
| Put | [api/{vaultName}/files/{changesetId}/finishadd](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BchangesetId%7D-finishadd~o-HttpPut.html) PUT: api/{vaultName}/files/{changesetId}/finishadd Finish of add file operation. This method adds files from changeset to the vault.   Adds files in the specified changeset to the vault. |
| Put | [api/{vaultName}/files/{changesetId}/upload](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BchangesetId%7D-upload~o-HttpPut.html) PUT: api/{vaultname}/files/{changesetId}/upload Upload file to changeset to add files operations   Uploads a changeset. |
| Put | [api/{vaultName}/files/{folderId}/new](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfolderId%7D-new~o-HttpPut.html) PUT: api/{vaultName}/files/{folderId}/new Add single file to vault   Adds a file to the specified folder in the specified vault. |
| Put | [api/stage/{vaultName}/{documentId}?folderId={folderId}&overrideVersion={overrideVersion}](PDM%20Pro%20API_ws~r-api-stage-%7BvaultName%7D-%7BdocumentId%7D-folderId%3D%7BfolderId%7D-overrideVersion%3D%7BoverrideVersion%7D~o-HttpPut.html) Checks in the specified document. |

See Also

[PDM Pro API Web Service](PDM%20Pro%20API_ws.html)