<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-files-{parentFolderId}~o-HttpPut.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Put | api/{vaultName}/files/{parentFolderId} |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [File Resource Group](PDM%20Pro%20API_ws~g-c98f0c35-a34d-4136-b9d9-0017d3189da7.html) : api/{vaultName}/files/{parentFolderId} (Put) |

Description

Adds a file to the specified folder.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| parentFolderId | (URI parameter) Parent folder ID (required) | integer |
| Id | (Response) ID of new file    Member of ObjectInfoShort model | integer |
| Name | (Response) Name of new file    Member of ObjectInfoShort model | string |
| Type | (Response) An ObjectType object; one of:     Folder = 0     File = 1     Bom = 3    Member of ObjectInfoShort model | ObjectType |
| Status | (Response) A StatusOperation object; one of:     Success = 0     Failure = 1    Member of ObjectInfoShort model | StatusOperation |
| Warning | (Response) A BaseWarningModel object that consists of:     Message (string)     IsBlocking (boolean)     IsError (boolean)    Member of ObjectInfoShort model | BaseWarningModel |

Response (application/json, text/json)

### Sample Data

```
[
  {
    "Id": 1,
    "Name": "sample string 2",
    "Type": 0,
    "Status": 0,
    "Warning": null
  },
  {
    "Id": 1,
    "Name": "sample string 2",
    "Type": 0,
    "Status": 0,
    "Warning": null
  }
]
```

Response (application/xml, text/xml)

### Sample Data

```
<ArrayOfObjectInfoShort xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <ObjectInfoShort>
    <Id>1</Id>
    <Name>sample string 2</Name>
    <Status>Success</Status>
    <Type>Folder</Type>
    <Warning i:nil="true" />
  </ObjectInfoShort>
  <ObjectInfoShort>
    <Id>1</Id>
    <Name>sample string 2</Name>
    <Status>Success</Status>
    <Type>Folder</Type>
    <Warning i:nil="true" />
  </ObjectInfoShort>
</ArrayOfObjectInfoShort>
```

Remarks

This operation can return an array of ObjectInfoShort objects.

See Also

[File Resource Group](PDM%20Pro%20API_ws~g-c98f0c35-a34d-4136-b9d9-0017d3189da7.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)