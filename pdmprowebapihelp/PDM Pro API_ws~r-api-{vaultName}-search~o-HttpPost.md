<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-search~o-HttpPost.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Post | api/{vaultName}/search |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Vault Resource Group](PDM%20Pro%20API_ws~g-fb61677a-af45-4e1b-a4a6-57412759c59e.html) : api/{vaultName}/search (Post) |

Description

Search vault

Gets objects in the vault that contain the specified string.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| Id | (Response) ID of vault object    Member of VaultObject model | integer |
| Type | (Response) An ObjectType; one of:     Folder = 0     File = 0     Bom = 0    Member of VaultObject model | ObjectType |

Request (application/json, text/json)

Body parameter contains the string to search the vault for

### Sample Data

```
"sample string 1"
```

Request (application/xml, text/xml)

Body parameter contains the string to search the vault for

### Sample Data

```
<string xmlns="http://schemas.microsoft.com/2003/10/Serialization/">sample string 1</string>
```

Request (application/x-www-form-urlencoded)

Response (application/json, text/json)

### Sample Data

```
[
  {
    "Id": 1,
    "Type": 0
  },
  {
    "Id": 1,
    "Type": 0
  }
]
```

Response (application/xml, text/xml)

### Sample Data

```
<ArrayOfVaultObject xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <VaultObject>
    <Id>1</Id>
    <Type>Folder</Type>
  </VaultObject>
  <VaultObject>
    <Id>1</Id>
    <Type>Folder</Type>
  </VaultObject>
</ArrayOfVaultObject>
```

Remarks

This operation:

* takes a body parameter that contains the string to search the vault for.* returns an array of VaultObjects.

See Also

[Vault Resource Group](PDM%20Pro%20API_ws~g-fb61677a-af45-4e1b-a4a6-57412759c59e.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)