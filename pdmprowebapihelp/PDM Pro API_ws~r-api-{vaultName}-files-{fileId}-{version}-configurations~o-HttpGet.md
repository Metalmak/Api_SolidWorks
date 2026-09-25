<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-files-{fileId}-{version}-configurations~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/files/{fileId}/{version}/configurations |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [File Resource Group](PDM%20Pro%20API_ws~g-20f0f203-5b33-4c77-baf6-4cccf91271c2.html) : api/{vaultName}/files/{fileId}/{version}/configurations (Get) |

Description

Get file configurations

Gets the configurations of the specified file.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| fileId | (URI parameter) File ID (required) | integer |
| version | (URI parameter) Version (required) | integer |
| ConfigurationName | (Response) Configuration name    Member of Config model | string |
| ConfigurationId | (Response) Configuration ID    Member of Config model | integer |

Response (application/json, text/json)

### Sample Data

```
[
  {
    "ConfigurationName": "sample string 1",
    "ConfigurationId": 2
  },
  {
    "ConfigurationName": "sample string 1",
    "ConfigurationId": 2
  }
]
```

Response (application/xml, text/xml)

### Sample Data

```
<ArrayOfConfig xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <Config>
    <ConfigurationId>2</ConfigurationId>
    <ConfigurationName>sample string 1</ConfigurationName>
  </Config>
  <Config>
    <ConfigurationId>2</ConfigurationId>
    <ConfigurationName>sample string 1</ConfigurationName>
  </Config>
</ArrayOfConfig>
```

Remarks

This operation returns an array of Config objects.

See Also

[File Resource Group](PDM%20Pro%20API_ws~g-20f0f203-5b33-4c77-baf6-4cccf91271c2.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)