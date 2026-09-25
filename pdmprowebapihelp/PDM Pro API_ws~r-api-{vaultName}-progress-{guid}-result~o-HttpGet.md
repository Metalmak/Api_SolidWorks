<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-progress-{guid}-result~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/progress/{guid}/result |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Progress Resource Group](PDM%20Pro%20API_ws~g-2279cdf6-53fe-4409-9acb-8511c5f37590.html) : api/{vaultName}/progress/{guid}/result (Get) |

Description

Get operation result

Gets the result of the specified operation.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| guid | (URI parameter) Operation GUID (required) | string |

Response (application/json, text/json)

### Sample Data

```
{}
```

Response (application/xml, text/xml)

### Sample Data

```
<z:anyType xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns:z="http://schemas.microsoft.com/2003/10/Serialization/" />
```

Remarks

The operation GUID can be found in the response of api/{vaultName}/files/{changesetId}/finishadd (Put).

See Also

[Progress Resource Group](PDM%20Pro%20API_ws~g-2279cdf6-53fe-4409-9acb-8511c5f37590.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)