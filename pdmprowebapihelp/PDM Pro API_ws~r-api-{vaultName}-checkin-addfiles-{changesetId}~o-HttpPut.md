<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-checkin-addfiles-{changesetId}~o-HttpPut.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Put | api/{vaultName}/checkin/addfiles/{changesetId} |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Stage Resource Group](PDM%20Pro%20API_ws~g-31fb4871-fcc6-41c5-8856-b0faf87b89f3.html) : api/{vaultName}/checkin/addfiles/{changesetId} (Put) |

Description

Upload files or document ids to changeset to the check in operation

Uploads files to the specified changeset for checkin.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| changesetId | (URI and response parameter) Changeset ID (URI required) | integer |
| References | (Response) Array of FileInfo objects; each FileInfo consists of:     File (File object that consists of:        FileId (integer)        FileName (string)     )     Folder (Folder object that consist of:        FolderId (integer)        FolderPath (string)     )     Version (integer)     Config (Config object that consists of:        ConfigurationName (string)        ConfigurationId (integer)     ) | Collection of FileInfo |

Response (application/json, text/json)

### Sample Data

```
{
  "ChangesetId": 1,
  "References": [
    {
      "File": {
        "FileId": 1,
        "FileName": "sample string 2"
      },
      "Folder": {
        "FolderId": 1,
        "FolderPath": "sample string 2"
      },
      "Version": 1,
      "Config": {
        "ConfigurationName": "sample string 1",
        "ConfigurationId": 2
      }
    },
    {
      "File": {
        "FileId": 1,
        "FileName": "sample string 2"
      },
      "Folder": {
        "FolderId": 1,
        "FolderPath": "sample string 2"
      },
      "Version": 1,
      "Config": {
        "ConfigurationName": "sample string 1",
        "ConfigurationId": 2
      }
    }
  ]
}
```

Response (application/xml, text/xml)

### Sample Data

```
<UploadModel xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <ChangesetId>1</ChangesetId>
  <References>
    <FileInfo>
      <Config>
        <ConfigurationId>2</ConfigurationId>
        <ConfigurationName>sample string 1</ConfigurationName>
      </Config>
      <File>
        <FileId>1</FileId>
        <FileName>sample string 2</FileName>
      </File>
      <Folder>
        <FolderId>1</FolderId>
        <FolderPath>sample string 2</FolderPath>
      </Folder>
      <Version>1</Version>
    </FileInfo>
    <FileInfo>
      <Config>
        <ConfigurationId>2</ConfigurationId>
        <ConfigurationName>sample string 1</ConfigurationName>
      </Config>
      <File>
        <FileId>1</FileId>
        <FileName>sample string 2</FileName>
      </File>
      <Folder>
        <FolderId>1</FolderId>
        <FolderPath>sample string 2</FolderPath>
      </Folder>
      <Version>1</Version>
    </FileInfo>
  </References>
</UploadModel>
```

See Also

[Stage Resource Group](PDM%20Pro%20API_ws~g-31fb4871-fcc6-41c5-8856-b0faf87b89f3.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)