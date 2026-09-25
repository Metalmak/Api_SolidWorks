<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-files-CheckOut~o-HttpPost.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Post | api/{vaultName}/files/CheckOut |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [File Resource Group](PDM%20Pro%20API_ws~g-20f0f203-5b33-4c77-baf6-4cccf91271c2.html) : api/{vaultName}/files/CheckOut (Post) |

Description

Lock file

Checks out the specified file.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| FileId | (Body and response parameter) File ID    Member of CheckOutResultModel model | integer |
| FolderId | (Body parameter) Folder ID | integer |
| IsSuccess | (Response) Whether the check out is successful    Member of CheckOutResultModel model | boolean |
| Warning | (Response) A BaseWarningModel object that consists of:     Message (string)     IsBlocking (boolean)     IsError (boolean)      Member of CheckOutResultModel model | Collection of BaseWarningModel |

Request (application/json, text/json)

### Sample Data

```
[
  {
    "FileId": 1,
    "FolderId": 2
  },
  {
    "FileId": 1,
    "FolderId": 2
  }
]
```

Request (application/xml, text/xml)

### Sample Data

```
<ArrayOfCheckOutItem xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <CheckOutItem>
    <FileId>1</FileId>
    <FolderId>2</FolderId>
  </CheckOutItem>
  <CheckOutItem>
    <FileId>1</FileId>
    <FolderId>2</FolderId>
  </CheckOutItem>
</ArrayOfCheckOutItem>
```

Request (application/x-www-form-urlencoded)

Response (application/json, text/json)

### Sample Data

```
[
  {
    "FileId": 1,
    "IsSuccess": true,
    "Warning": null
  },
  {
    "FileId": 1,
    "IsSuccess": true,
    "Warning": null
  }
]
```

Response (application/xml, text/xml)

### Sample Data

```
<ArrayOfCheckOutResultModel xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <CheckOutResultModel>
    <FileId>1</FileId>
    <IsSuccess>true</IsSuccess>
    <Warning i:nil="true" />
  </CheckOutResultModel>
  <CheckOutResultModel>
    <FileId>1</FileId>
    <IsSuccess>true</IsSuccess>
    <Warning i:nil="true" />
  </CheckOutResultModel>
</ArrayOfCheckOutResultModel>
```

Remarks

This operation returns the file ID, IsSuccess, and Warning.

See Also

[File Resource Group](PDM%20Pro%20API_ws~g-20f0f203-5b33-4c77-baf6-4cccf91271c2.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)