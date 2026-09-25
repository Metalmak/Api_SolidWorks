<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-folders-{folderId}-browse~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/folders/{folderId}/browse |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Folder Resource Group](PDM%20Pro%20API_ws~g-7b7f55f5-e86c-42e9-b881-27010dbf573a.html) : api/{vaultName}/folders/{folderId}/browse (Get) |

Description

Get browse folder

Gets the files and folders in the specified folder.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault  name (required) | string |
| folderId | (URI parameter) ID of folder in which to browse (required) | integer |
| Id | (Response) ID of object    Member of ObjectInfo model | integer |
| Name | (Response) Name of object    Member of ObjectInfo model | string |
| Size | (Response) Size of object    Member of ObjectInfo model | integer |
| ModifiedDate | (Response) Modification date    Member of ObjectInfo model | date |
| Version | (Response) Version    Member of ObjectInfo model | integer |
| State | (Response) State    Member of ObjectInfo model | string |
| StateId | (Response) State ID    Member of ObjectInfo model | integer |
| ParentFolderId | (Response) Parent folder ID    Member of ObjectInfo model | integer |
| Path | (Response) Folder path    Member of ObjectInfo model | string |
| Type | (Response) An ObjectType; one of:     Folder = 0     File = 1     Bom = 3    Member of ObjectInfo model | ObjectType |
| IsLocked | (Response) Whether the object is locked    Member of ObjectInfo model | integer |
| LockedBy | (Response) Locked by user    Member of ObjectInfo model | integer |
| IsShared | (Response) Whether the object is shared    Member of ObjectInfo model | integer |
| IsToolbox | (Response) Whether the object is in the toolbox    Member of ObjectInfo model | integer |
| IsDeleted | (Response) Whether the object is deleted    Member of ObjectInfo model | integer |

Response (application/json, text/json)

### Sample Data

```
[
  {
    "Id": 1,
    "Name": "sample string 2",
    "Size": 3,
    "ModifiedDate": "2022-05-27T09:24:09.3983559-04:00",
    "Version": 5,
    "State": "sample string 6",
    "StateId": 7,
    "ParentFolderId": 8,
    "Path": "sample string 9",
    "Type": 0,
    "IsLocked": 10,
    "LockedBy": 11,
    "IsShared": 12,
    "IsToolbox": 13,
    "IsDeleted": 14
  },
  {
    "Id": 1,
    "Name": "sample string 2",
    "Size": 3,
    "ModifiedDate": "2022-05-27T09:24:09.3983559-04:00",
    "Version": 5,
    "State": "sample string 6",
    "StateId": 7,
    "ParentFolderId": 8,
    "Path": "sample string 9",
    "Type": 0,
    "IsLocked": 10,
    "LockedBy": 11,
    "IsShared": 12,
    "IsToolbox": 13,
    "IsDeleted": 14
  }
]
```

Response (application/xml, text/xml)

### Sample Data

```
<ArrayOfObjectInfo xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <ObjectInfo>
    <Id>1</Id>
    <IsDeleted>14</IsDeleted>
    <IsLocked>10</IsLocked>
    <IsShared>12</IsShared>
    <IsToolbox>13</IsToolbox>
    <LockedBy>11</LockedBy>
    <ModifiedDate>2022-05-27T09:24:09.3983559-04:00</ModifiedDate>
    <Name>sample string 2</Name>
    <ParentFolderId>8</ParentFolderId>
    <Path>sample string 9</Path>
    <Size>3</Size>
    <State>sample string 6</State>
    <StateId>7</StateId>
    <Type>Folder</Type>
    <Version>5</Version>
  </ObjectInfo>
  <ObjectInfo>
    <Id>1</Id>
    <IsDeleted>14</IsDeleted>
    <IsLocked>10</IsLocked>
    <IsShared>12</IsShared>
    <IsToolbox>13</IsToolbox>
    <LockedBy>11</LockedBy>
    <ModifiedDate>2022-05-27T09:24:09.3983559-04:00</ModifiedDate>
    <Name>sample string 2</Name>
    <ParentFolderId>8</ParentFolderId>
    <Path>sample string 9</Path>
    <Size>3</Size>
    <State>sample string 6</State>
    <StateId>7</StateId>
    <Type>Folder</Type>
    <Version>5</Version>
  </ObjectInfo>
</ArrayOfObjectInfo>
```

Example

See the example for [api/{vaultName}/authenticate](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-authenticate~o-HttpPost.html).

Remarks

This operation returns an array of ObjectInfo objects.

See Also

[Folder Resource Group](PDM%20Pro%20API_ws~g-7b7f55f5-e86c-42e9-b881-27010dbf573a.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)