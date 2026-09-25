<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-info~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/info |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Vault Resource Group](PDM%20Pro%20API_ws~g-fb61677a-af45-4e1b-a4a6-57412759c59e.html) : api/{vaultName}/info (Get) |

Description

Get vault properties

Gets the properties of the specified vault.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| Version | (Response) Vault version    Member of VaultProp model | integer |
| VaultType | (Response) Type of vault      Member of VaultProp model | string |
| ArchiveServer | (Response) Archive server      Member of VaultProp model | string |
| DatabaseName | (Response) Database name      Member of VaultProp model | string |
| DatabaseServer | (Response) Database server      Member of VaultProp model | string |
| VaultID | (Response) Vault ID      Member of VaultProp model | globally unique identifier |

Response (application/json, text/json)

### Sample Data

```
{
  "Version": 1,
  "VaultType": "sample string 2",
  "ArchiveServer": "sample string 3",
  "DatabaseName": "sample string 4",
  "DatabaseServer": "sample string 5",
  "VaultID": "cad69219-245c-4410-9e2a-862ea8e8f933"
}
```

Response (application/xml, text/xml)

### Sample Data

```
<VaultProp xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <ArchiveServer>sample string 3</ArchiveServer>
  <DatabaseName>sample string 4</DatabaseName>
  <DatabaseServer>sample string 5</DatabaseServer>
  <VaultID>cad69219-245c-4410-9e2a-862ea8e8f933</VaultID>
  <VaultType>sample string 2</VaultType>
  <Version>1</Version>
</VaultProp>
```

See Also

[Vault Resource Group](PDM%20Pro%20API_ws~g-fb61677a-af45-4e1b-a4a6-57412759c59e.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)