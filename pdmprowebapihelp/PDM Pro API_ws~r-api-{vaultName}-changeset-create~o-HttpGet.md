<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-changeset-create~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/changeset/create |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Stage Resource Group](PDM%20Pro%20API_ws~g-31fb4871-fcc6-41c5-8856-b0faf87b89f3.html) : api/{vaultName}/changeset/create (Get) |

Description

Generate changesetId

Gets a changeset ID for the specified vault.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |

Response (application/json, text/json)

Returns the new changeset ID

### Sample Data

```
1
```

Response (application/xml, text/xml)

Returns the new changeset ID

### Sample Data

```
<int xmlns="http://schemas.microsoft.com/2003/10/Serialization/">1</int>
```

See Also

[Stage Resource Group](PDM%20Pro%20API_ws~g-31fb4871-fcc6-41c5-8856-b0faf87b89f3.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)