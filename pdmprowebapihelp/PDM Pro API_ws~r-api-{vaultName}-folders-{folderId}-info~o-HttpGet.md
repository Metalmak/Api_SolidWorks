<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-folders-{folderId}-info~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/folders/{folderId}/info |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Folder Resource Group](PDM%20Pro%20API_ws~g-7b7f55f5-e86c-42e9-b881-27010dbf573a.html) : api/{vaultName}/folders/{folderId}/info (Get) |

Description

Get folder info

Gets information for the specified folder.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| folderId | (URI parameter) Folder ID (required) | integer |
| Folder | (Response) A Folder object that consists of:     FolderId (integer)     FolderPath (string)    Member of FolderInfo model | Folder |
| FolderName | (Response) Folder name    Member of FolderInfo model | string |
| ParentFolderId | (Response) Parent folder ID    Member of FolderInfo model | integer |

Response (application/json, text/json)

### Sample Data

```
{
  "Folder": {
    "FolderId": 1,
    "FolderPath": "sample string 2"
  },
  "FolderName": "sample string 1",
  "ParentFolderId": 2
}
```

Response (application/xml, text/xml)

### Sample Data

```
<FolderInfo xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <Folder>
    <FolderId>1</FolderId>
    <FolderPath>sample string 2</FolderPath>
  </Folder>
  <FolderName>sample string 1</FolderName>
  <ParentFolderId>2</ParentFolderId>
</FolderInfo>
```

See Also

[Folder Resource Group](PDM%20Pro%20API_ws~g-7b7f55f5-e86c-42e9-b881-27010dbf573a.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)