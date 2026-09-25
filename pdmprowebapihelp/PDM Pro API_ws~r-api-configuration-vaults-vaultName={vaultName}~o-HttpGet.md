<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-configuration-vaults-vaultName={vaultName}~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/configuration/vaults?vaultName={vaultName} |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Configuration Resource Group](PDM%20Pro%20API_ws~g-7320ff77-ab40-4885-b6b1-f53a97cc4f2f.html) : api/configuration/vaults?vaultName={vaultName} (Get) |

Description

Get all vaults from the config file

Gets all vaults from the vault configuration file.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (default is empty string) | string |
| Name | (Response) Vault name matching regular expression pattern: ^[^|\\/:\*?"<>|]+$    Member of VaultProperties model  See the **Remarks**. | string |
| DatabaseName | (Response) Database name matching regular expression pattern: ^[^|\\/:\*?"<>|]+$    Member of VaultProperties model  See the **Remarks**. | string |
| ArchiveServer | Archive server name    Member of VaultProperties model  See the **Remarks**. | string |
| ArchiveServerPort | Archive server port    Member of VaultProperties model  See the **Remarks**. | integer |
| DatabaseServer | Database server    Member of VaultProperties model  See the **Remarks**. | string |
| CommandTimeOut | Length before time out (seconds)    Member of VaultProperties model  See the **Remarks**. | integer |
| IndexingUserId | Indexing user ID    Member of VaultProperties model  See the **Remarks**. | integer |

Response (application/json, text/json)

### Sample Data

```
[
  {
    "Name": "sample string 1",
    "DatabaseName": "sample string 2",
    "ArchiveServer": "sample string 3",
    "ArchiveServerPort": 4,
    "DatabaseServer": "sample string 5",
    "CommandTimeOut": 6,
    "IndexingUserId": 7
  },
  {
    "Name": "sample string 1",
    "DatabaseName": "sample string 2",
    "ArchiveServer": "sample string 3",
    "ArchiveServerPort": 4,
    "DatabaseServer": "sample string 5",
    "CommandTimeOut": 6,
    "IndexingUserId": 7
  }
]
```

Response (application/xml, text/xml)

### Sample Data

```
<ArrayOfVaultProperties xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Configuration">
  <VaultProperties>
    <ArchiveServer>sample string 3</ArchiveServer>
    <ArchiveServerPort>4</ArchiveServerPort>
    <CommandTimeOut>6</CommandTimeOut>
    <DatabaseName>sample string 2</DatabaseName>
    <DatabaseServer>sample string 5</DatabaseServer>
    <IndexingUserId>7</IndexingUserId>
    <Name>sample string 1</Name>
  </VaultProperties>
  <VaultProperties>
    <ArchiveServer>sample string 3</ArchiveServer>
    <ArchiveServerPort>4</ArchiveServerPort>
    <CommandTimeOut>6</CommandTimeOut>
    <DatabaseName>sample string 2</DatabaseName>
    <DatabaseServer>sample string 5</DatabaseServer>
    <IndexingUserId>7</IndexingUserId>
    <Name>sample string 1</Name>
  </VaultProperties>
</ArrayOfVaultProperties>
```

Remarks

This operation can return an array of VaultProperties objects. See the Response samples.

See Also

[Configuration Resource Group](PDM%20Pro%20API_ws~g-7320ff77-ab40-4885-b6b1-f53a97cc4f2f.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)