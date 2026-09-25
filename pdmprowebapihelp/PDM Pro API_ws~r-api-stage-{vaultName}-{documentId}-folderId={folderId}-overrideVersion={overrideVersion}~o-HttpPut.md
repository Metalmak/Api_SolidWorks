<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-stage-{vaultName}-{documentId}-folderId={folderId}-overrideVersion={overrideVersion}~o-HttpPut.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Put | api/stage/{vaultName}/{documentId}?folderId={folderId}&overrideVersion={overrideVersion} |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Stage Resource Group](PDM%20Pro%20API_ws~g-e97ee2e8-3e51-4fe9-991a-ddc5b293f468.html) : api/stage/{vaultName}/{documentId}?folderId={folderId}&overrideVersion={overrideVersion} (Put) |

Description

Checks in the specified document.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| documentId | (URI parameter) Document ID (required) | integer |
| folderId | (URI parameter) Folder ID (default is 0) | integer |
| overrideVersion | (URI parameter) Whether to override the current versions of files (default value is false) | boolean |

Response (application/json, text/json)

True if checkin is successful, false if not

### Sample Data

```
true
```

Response (application/xml, text/xml)

True if checkin is successful, false if not

### Sample Data

```
<boolean xmlns="http://schemas.microsoft.com/2003/10/Serialization/">true</boolean>
```

See Also

[Stage Resource Group](PDM%20Pro%20API_ws~g-e97ee2e8-3e51-4fe9-991a-ddc5b293f468.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)