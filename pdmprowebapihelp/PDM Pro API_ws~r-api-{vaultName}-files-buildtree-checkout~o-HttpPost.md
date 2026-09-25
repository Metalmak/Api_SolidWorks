<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-files-buildtree-checkout~o-HttpPost.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Post | api/{vaultName}/files/buildtree/checkout |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [File Resource Group](PDM%20Pro%20API_ws~g-20f0f203-5b33-4c77-baf6-4cccf91271c2.html) : api/{vaultName}/files/buildtree/checkout (Post) |

Description

Build checkout references tree

Gets the tree of references in the specified file's checkout.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Valut name (required) | string |
| FileId | (Body parameter) File ID    Member of CheckOutItem; see **Remarks** | integer |
| FolderId | (Body parameter) Folder ID    Member of CheckOutItem; see **Remarks** | integer |
| File | (Response) A FileInfoConfigLess object that consists of:     File (File object consists of:        FileId (integer)        FileName (string)    )     Folder (Folder object consists of:        FolderId (integer)        FolderPath (string)    )     Version (integer)    Member of FileRefOfFileInfoConfigLess model; see **Remarks** | FileInfoConfigLess |
| IsToolbox | (Response) Whether is a toolbox item    Member of FileRefOfFileInfoConfigLess model; see **Remarks** | integer |
| ObjectType | (Response) PweObjectType model; one of:     ObjType\_NoObject = 0     ObjType\_File = 1     ObjType\_InternalComponent = 2     ObjType\_SavedBOM = 3     ObjType\_Item = 4     ObjType\_CutListItem = 5    Member of FileRefOfFileInfoConfigLess model; see **Remarks** | String |

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

Response (application/json)

Response (text/json)

Response (application/xml)

Response (text/xml)

Remarks

This operation can:

* take an array of CheckOutItem objects. Each CheckOutItem consists of FileId and Folder Id.* return an array of FileRefOfFileInfoConfigLess objects that represent the tree of references to include in the file's checkout.

See Also

[File Resource Group](PDM%20Pro%20API_ws~g-20f0f203-5b33-4c77-baf6-4cccf91271c2.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)