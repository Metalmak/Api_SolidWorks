<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-files-{folderId}-new~o-HttpPut.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Put | api/{vaultName}/files/{folderId}/new |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Stage Resource Group](PDM%20Pro%20API_ws~g-e97ee2e8-3e51-4fe9-991a-ddc5b293f468.html) : api/{vaultName}/files/{folderId}/new (Put) |

Description

PUT: api/{vaultName}/files/{folderId}/new Add single file to vault

Adds a file to the specified folder in the specified vault.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| folderId | (URI and response parameter) Folder ID (required) | integer |
| DocumentId | (Response) Document ID | integer |
| FileName | (Response) File name | string |
| VaultPath | (Response) Vault path | string |
| Warning | (Response) A BaseWarningModel object that consists of:     Message (string)     IsBlocking (boolean)     IsError (boolean) | Collection of BaseWarningModel |

Response (application/json, text/json)

### Sample Data

```
{
  "DocumentId": 1,
  "FolderId": 2,
  "FileName": "sample string 3",
  "VaultPath": "sample string 4",
  "Warning": null
}
```

Response (application/xml, text/xml)

### Sample Data

```
<AddDocumentResultModel xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <DocumentId>1</DocumentId>
  <FileName>sample string 3</FileName>
  <FolderId>2</FolderId>
  <VaultPath>sample string 4</VaultPath>
  <Warning i:nil="true" />
</AddDocumentResultModel>
```

See Also

[Stage Resource Group](PDM%20Pro%20API_ws~g-e97ee2e8-3e51-4fe9-991a-ddc5b293f468.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)